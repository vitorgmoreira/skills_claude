# 📦 Guia de Instalação e Ativação

## 🎯 Como Ativar a Skill pdf-to-skill-converter

### Opção 1: Instalação Manual (Recomendada)

1. **Copie toda a pasta para o diretório de skills do usuário:**

```bash
cp -r /mnt/user-data/outputs/pdf-to-skill-converter /mnt/skills/user/
```

2. **Verifique a instalação:**

```bash
ls -la /mnt/skills/user/pdf-to-skill-converter/
```

Deve mostrar:
```
SKILL.md
README.md
modules/
templates/
config/
examples/
```

3. **Teste a skill:**

Pergunte ao Claude:
```
"Claude, você tem acesso à skill pdf-to-skill-converter?"
```

Claude deve responder confirmando e explicando o que a skill faz.

---

### Opção 2: Via Interface (se disponível)

1. Acesse Settings > Skills
2. Click em "Add Custom Skill"
3. Selecione a pasta `/mnt/user-data/outputs/pdf-to-skill-converter`
4. Confirme instalação

---

## 📚 Preparando PDFs para Conversão

### Requisitos do PDF

✅ **PDFs compatíveis:**
- Texto extraível (não escaneado)
- Estrutura com capítulos/seções
- Formato técnico/business (não ficção)
- Tamanho: 50-1000 páginas ideal

⚠️ **PDFs com limitações:**
- PDFs escaneados (OCR pode degradar qualidade)
- Livros sem estrutura clara
- Ficção ou narrativa (menos útil)
- PDFs protegidos com senha

### Upload do PDF

1. **Coloque o PDF na pasta de uploads:**

```bash
# Via interface: faça upload normalmente
# Via CLI: copie para a pasta
cp seu-livro.pdf /mnt/user-data/uploads/
```

2. **Verifique que está acessível:**

```bash
ls -la /mnt/user-data/uploads/seu-livro.pdf
```

---

## 🚀 Primeira Conversão

### Passo a Passo

1. **Certifique-se que o PDF está em uploads**

2. **Solicite a conversão:**

```
"Claude, use a skill pdf-to-skill-converter para processar 
[nome-do-arquivo.pdf] e criar uma skill especializada"
```

3. **Escolha o modo quando solicitado:**
   - Modo Básico (0 tokens)
   - Modo Premium (investimento inicial, ROI rápido)

4. **Aguarde o processamento:**
   - Básico: 2-5 minutos
   - Premium: 10-20 minutos

5. **Skill gerada em:**
   ```
   /mnt/user-data/outputs/[nome-do-livro]-skill/
   ```

---

## 📍 Ativando Skills Geradas

### Para Uso Temporário

Skills em `/mnt/user-data/outputs/` são acessíveis mas temporárias.

### Para Uso Permanente

Mova a skill gerada para o diretório de skills do usuário:

```bash
cp -r /mnt/user-data/outputs/revenue-architecture-skill /mnt/skills/user/
```

Agora a skill estará sempre disponível!

---

## 🔧 Dependências Python

A skill conversor usa as seguintes bibliotecas Python:

### Instaladas (nativas)
- `re` (regex)
- `json`
- `pathlib`
- `typing`

### Necessárias (instalar se ausente)

```bash
pip install pdfplumber --break-system-packages
pip install anthropic --break-system-packages  # Opcional, para Modo Premium
```

**Verificar instalação:**

```bash
python3 -c "import pdfplumber; print('pdfplumber OK')"
```

---

## ✅ Checklist de Instalação

Use esta checklist para garantir que tudo está funcionando:

- [ ] Skill pdf-to-skill-converter copiada para `/mnt/skills/user/`
- [ ] SKILL.md acessível em `/mnt/skills/user/pdf-to-skill-converter/SKILL.md`
- [ ] Claude reconhece a skill quando perguntado
- [ ] pdfplumber instalado (`python3 -c "import pdfplumber"`)
- [ ] PDF de teste disponível em `/mnt/user-data/uploads/`
- [ ] Primeira conversão teste executada com sucesso
- [ ] Skill gerada acessível e funcional

---

## 🧪 Teste Completo

Execute este teste para validar instalação completa:

### 1. Verificar Skill Conversor

```
"Claude, você tem a skill pdf-to-skill-converter? Se sim, 
explique brevemente o que ela faz."
```

**Resposta esperada:** Claude explica que pode converter PDFs em skills.

### 2. Teste com PDF Pequeno

Faça upload de um PDF pequeno (10-50 páginas) e converta em Modo Básico:

```
"Converta [teste.pdf] em skill usando Modo Básico"
```

**Resultado esperado:** Conversão completa em 2-3 minutos, 0 tokens.

### 3. Testar Skill Gerada

```
"Claude, você tem a skill [teste]? Se sim, responda uma 
pergunta sobre o conteúdo: [pergunta específica]"
```

**Resultado esperado:** Claude responde baseado no conteúdo do livro.

---

## 🐛 Troubleshooting

### Problema: Claude não reconhece a skill

**Solução:**
1. Verifique que SKILL.md está em `/mnt/skills/user/pdf-to-skill-converter/`
2. Reinicie a conversa
3. Pergunte explicitamente: "Use a skill pdf-to-skill-converter"

### Problema: Erro ao processar PDF

**Possíveis causas:**
- PDF protegido → Remova proteção
- PDF escaneado → Use OCR ou PDF com texto
- Arquivo corrompido → Redownload do PDF

**Solução:**
```bash
# Verifique que o PDF é válido
python3 -c "import pdfplumber; pdfplumber.open('caminho/arquivo.pdf')"
```

### Problema: pdfplumber não encontrado

**Solução:**
```bash
pip install pdfplumber --break-system-packages
```

### Problema: Conversão muito lenta

**Causas comuns:**
- PDF muito grande (>1000 páginas)
- Modo Premium com muitos capítulos
- Processamento de tabelas complexas

**Solução:**
- Use Modo Básico para PDFs gigantes
- Seja paciente com Premium (qualidade vale a pena)
- Considere dividir PDFs muito grandes

### Problema: Skill gerada não responde bem

**Diagnóstico:**
1. Verifique SKILL.md foi gerado
2. Verifique que capítulos foram criados
3. Teste com perguntas mais específicas

**Melhoria:**
- Reconverta em Modo Premium para melhor qualidade
- Adicione mais contexto nas perguntas
- Especifique capítulos quando souber

---

## 📊 Monitoramento de Uso

### Verificar Skills Ativas

```bash
ls -la /mnt/skills/user/
```

### Verificar Skills Geradas

```bash
ls -la /mnt/user-data/outputs/ | grep "-skill"
```

### Estatísticas de uma Skill

Abra o `metadata.json` de qualquer skill gerada:

```bash
cat /mnt/user-data/outputs/[nome-skill]/metadata.json | python3 -m json.tool
```

---

## 🔄 Atualizações

### Atualizando a Skill Conversor

Quando houver nova versão:

```bash
# Backup da versão antiga
mv /mnt/skills/user/pdf-to-skill-converter /mnt/skills/user/pdf-to-skill-converter.backup

# Instalar nova versão
cp -r /nova/versao/pdf-to-skill-converter /mnt/skills/user/
```

### Reconvertendo um Livro

Para reconverter com melhorias:

1. PDF já está em uploads
2. Solicite conversão novamente
3. Escolha modo diferente ou mesmo modo
4. Substitua skill antiga pela nova

---

## 📚 Recursos Adicionais

### Documentação
- `SKILL.md` - Documentação técnica completa
- `README.md` - Guia rápido de uso
- `examples/` - Exemplos de interação

### Suporte
- Pergunte ao Claude sobre funcionalidades específicas
- Consulte `SKILL.md` para casos de uso avançados
- Teste com PDFs pequenos primeiro

---

## 🎯 Próximos Passos Recomendados

Após instalação bem-sucedida:

1. ✅ **Converta seu primeiro livro** (escolha um importante)
2. ✅ **Teste a skill gerada** com perguntas variadas
3. ✅ **Avalie Básico vs Premium** (tente ambos se possível)
4. ✅ **Crie biblioteca de skills** (converta múltiplos livros)
5. ✅ **Compartilhe com o time** (copie skills para outros usuários)
6. ✅ **Otimize workflow** (integre skills no dia a dia)

---

**🎉 Instalação completa! Você agora pode transformar qualquer livro em um especialista virtual!**

*Versão: 1.0.0 | Atualizado: 2025-10-27*
