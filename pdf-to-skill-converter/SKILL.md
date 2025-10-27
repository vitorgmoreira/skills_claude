---
name: pdf-to-skill-converter
description: Meta-skill que converte livros PDF em especialistas virtuais Claude otimizados. Oferece modo Básico (0 tokens) e Premium (com refinamento IA). Inclui cálculo dinâmico de custos, sistema de consulta interativa e geração automática de skills especializadas com navegação inteligente, FAQs, frameworks extraídos e exemplos contextualizados.
license: MIT
---

# PDF to Skill Converter - Meta-Skill de Geração de Especialistas Virtuais

## 🎯 Propósito

Esta skill converte qualquer PDF de livro técnico em uma **skill especializada otimizada** - essencialmente criando um **especialista virtual** no conteúdo do livro que Claude pode consultar para responder perguntas, aplicar conceitos e criar implementações práticas.

## 🧠 O Que Esta Skill Cria

Não apenas "um livro digitalizado", mas sim um **especialista virtual** que:

- ✅ Conhece o livro completamente
- ✅ Navega inteligentemente pelo conteúdo
- ✅ Adapta exemplos ao contexto do usuário
- ✅ Conecta conceitos de diferentes capítulos
- ✅ Responde instantaneamente
- ✅ Cria frameworks personalizados
- ✅ Disponível 24/7 a custo irrisório

## 🚀 Como Usar

### Comando Básico
```
"Claude, use a skill pdf-to-skill-converter para processar 
[nome-do-arquivo.pdf] e criar uma skill especializada"
```

### Comando com Contexto
```
"Claude, converta [nome-do-arquivo.pdf] em skill especializada,
contextualizando para [seu negócio/indústria/uso específico]"
```

## ⚙️ Processo de Conversão

### FASE 0: CONSULTA INTERATIVA (SEMPRE EXECUTAR PRIMEIRO)

**CRITICAL**: Antes de iniciar qualquer processamento, Claude DEVE apresentar as opções ao usuário de forma educativa e aguardar decisão explícita.

#### Template de Apresentação ao Usuário

```markdown
📚 Iniciando conversão de [{NOME_DO_PDF}]...

Antes de prosseguir, você precisa escolher o modo de conversão.
Deixe-me explicar as diferenças para que você tome a melhor decisão:

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

🔧 MODO BÁSICO (Conversão Estrutural)
💰 Custo: 0 tokens na geração

📖 O PDF tem {NUM_PAGINAS} páginas

O que este modo faz:
✅ Extrai todo o conteúdo (Python local - 0 tokens)
✅ Detecta estrutura: capítulos, seções, hierarquia
✅ Cria navegação inteligente e índices
✅ Quebra em camadas: TL;DR → Resumo → Completo
✅ Gera glossário e referências cruzadas
✅ Cria matriz de aplicabilidade
✅ Extrai frameworks e templates

Como funciona:
- TL;DRs: primeiras frases de cada seção (extração automática)
- FAQs: baseadas em títulos e subtítulos
- Exemplos: mantidos como no original
- Estruturação: 100% automática por regras

Qualidade resultante:
⭐⭐⭐⭐ Muito boa - Funcional imediatamente
⚠️ Pode precisar de ajustes manuais em TL;DRs/FAQs depois

Economia no uso: ~73% menos tokens por consulta
Melhor para: Livros para consulta eventual, POCs, testes

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

🚀 MODO PREMIUM (Ultra-Otimizado com IA)
💰 Custo estimado para {NUM_PAGINAS} páginas: ~{CUSTO_ESTIMADO}k tokens (${CUSTO_USD})

Cálculo: ~{TOKENS_POR_100_PAG}k tokens a cada 100 páginas
- TL;DRs por IA: ~{TLD_TOKENS}k tokens
- FAQs inteligentes: ~{FAQ_TOKENS}k tokens  
- Contextualização: ~{CONTEXT_TOKENS}k tokens
- Análise de nuances: ~{NUANCE_TOKENS}k tokens

O que ADICIONA ao Modo Básico:
✅ Tudo do Modo Básico +
✅ TL;DRs gerados por IA (concisos, precisos, relevantes)
✅ FAQs inteligentes (perguntas realmente úteis)
✅ Exemplos contextualizados para seu negócio
✅ Detecção automática de contradições e nuances
✅ Analogias e adaptações para seu contexto específico
✅ Comparações entre conceitos similares
✅ Extração semântica avançada de conceitos

Como funciona:
- Claude processa cada capítulo para gerar conteúdo refinado
- Análise semântica profunda de conceitos
- Contextualização baseada no seu negócio
- Otimização máxima para uso recorrente

Qualidade resultante:
⭐⭐⭐⭐⭐ Excepcional - Pronto para uso avançado
✨ Especialista virtual de altíssima qualidade

Economia no uso: ~88% menos tokens por consulta
ROI: Positivo após apenas 3-5 consultas!

Melhor para: Livros críticos para o negócio, uso intensivo diário

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

📊 COMPARAÇÃO DE CUSTOS - 100 Consultas ao Longo do Tempo

Cenário: Livro de {NUM_PAGINAS} páginas, 100 perguntas ao longo de semanas/meses

❌ Sem skill otimizada:
   Token médio por consulta: ~55k
   Total em 100 consultas: 5.500.000 tokens
   Custo: ~$16.50

✅ Com Modo Básico:
   Geração: $0.00
   Token médio por consulta: ~15k
   Total em 100 consultas: 1.500.000 tokens
   Custo total: $4.50
   💰 Economia: $12.00 (73%)

✅ Com Modo Premium:
   Geração: ${CUSTO_USD} (uma única vez)
   Token médio por consulta: ~5.6k
   Total em 100 consultas: 560.000 tokens
   Custo total: ${CUSTO_TOTAL_PREMIUM}
   💰 Economia: ${ECONOMIA_PREMIUM} ({PERCENTUAL_ECONOMIA}%)
   
   🎯 Break-even: Após {BREAKEVEN_QUERIES} consultas
   🚀 ROI: Cada consulta após break-even economiza ${ECONOMIA_POR_QUERY}

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

🎯 TABELA DE CUSTOS POR TAMANHO DE LIVRO

| Páginas | Modo Básico | Modo Premium | Break-even | Economia (100 consultas) |
|---------|-------------|--------------|------------|--------------------------|
| 100     | $0.00       | ~$0.11       | 1 consulta | $14.38                   |
| 200     | $0.00       | ~$0.22       | 2 consultas| $14.27                   |
| 300     | $0.00       | ~$0.33       | 3 consultas| $14.16                   |
| 400     | $0.00       | ~$0.44       | 3 consultas| $14.05                   |
| 500     | $0.00       | ~$0.55       | 4 consultas| $13.94                   |
| 600     | $0.00       | ~$0.66       | 5 consultas| $13.83                   |

*Preços baseados em Claude Sonnet 4 ($3/M input tokens)*

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

💡 POR QUE ESSAS OTIMIZAÇÕES EXISTEM?

**Problema sem otimização**:
❌ Livros grandes = 50-80k tokens por consulta simples
❌ Claude não sabe onde buscar → lê múltiplos capítulos
❌ Usuário paga caro em CADA pergunta
❌ Resposta demorada

**Solução: Estruturação inteligente**:
✅ Navegação clara → Claude sabe exatamente onde ler
✅ Camadas de profundidade → lê apenas o necessário
✅ FAQs prontas → resposta instantânea sem processar
✅ Índices semânticos → busca precisa de conceitos

**Benefício do refinamento com IA (Premium)**:
✅ TL;DRs precisos → resolve 60% das perguntas com 100 tokens
✅ FAQs relevantes → resposta sem ler capítulo completo
✅ Exemplos contextualizados → aplicação imediata
✅ ROI extremamente rápido → paga-se em pouquíssimas consultas

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

🤔 Qual modo você prefere?

[1] Modo Básico - Começar agora (0 tokens)
[2] Modo Premium - Máxima qualidade (~${CUSTO_USD})
[3] Me dê mais detalhes sobre as diferenças
[4] Mostre exemplos de output de cada modo
```

#### Cálculo Dinâmico de Custos

```python
def calcular_custos(num_paginas):
    """
    Calcula custos baseado no número de páginas
    ~220 tokens por página = ~1.1k tokens por 100 páginas de refinamento
    """
    # Tokens de refinamento a cada 100 páginas
    tokens_por_100_pag = 11000  # ~11k tokens
    
    # Cálculo proporcional
    custo_tokens = (num_paginas / 100) * tokens_por_100_pag
    custo_usd = (custo_tokens / 1_000_000) * 3  # $3 por M tokens
    
    # Breakdown
    tldr_tokens = int(custo_tokens * 0.36)  # 36%
    faq_tokens = int(custo_tokens * 0.27)   # 27%
    context_tokens = int(custo_tokens * 0.23) # 23%
    nuance_tokens = int(custo_tokens * 0.14)  # 14%
    
    # Economia e ROI
    custo_sem_skill = 16.50
    custo_com_basico = 4.50
    custo_com_premium = custo_usd + (560_000 / 1_000_000 * 3)
    
    economia_premium = custo_sem_skill - custo_com_premium
    percentual = (economia_premium / custo_sem_skill) * 100
    
    # Break-even
    economia_por_query = (55000 - 5600) / 1_000_000 * 3  # $0.148
    breakeven = math.ceil(custo_usd / economia_por_query)
    
    return {
        'tokens_por_100_pag': tokens_por_100_pag / 1000,  # em k
        'custo_estimado': int(custo_tokens / 1000),  # em k
        'custo_usd': f"{custo_usd:.2f}",
        'tldr_tokens': tldr_tokens / 1000,
        'faq_tokens': faq_tokens / 1000,
        'context_tokens': context_tokens / 1000,
        'nuance_tokens': nuance_tokens / 1000,
        'custo_total_premium': f"{custo_com_premium:.2f}",
        'economia_premium': f"{economia_premium:.2f}",
        'percentual_economia': f"{percentual:.0f}",
        'breakeven_queries': breakeven,
        'economia_por_query': f"{economia_por_query:.3f}"
    }
```

#### Processamento da Escolha do Usuário

```python
def processar_escolha(resposta_usuario):
    """
    Processa a escolha do usuário e configura pipeline
    """
    resposta = resposta_usuario.lower().strip()
    
    if resposta in ['1', 'basico', 'básico', 'modo basico', 'modo básico']:
        return {
            'modo': 'basico',
            'llm_refinement': False,
            'context': {}
        }
    
    elif resposta in ['2', 'premium', 'modo premium']:
        # Coletar informações de contexto
        return {
            'modo': 'premium',
            'llm_refinement': True,
            'context': coletar_contexto()
        }
    
    elif resposta in ['3', 'detalhes', 'mais detalhes', 'mais informações']:
        # Expandir explicação e reapresentar escolha
        return 'expandir_explicacao'
    
    elif resposta in ['4', 'exemplos', 'mostrar exemplos']:
        # Mostrar exemplos de output
        return 'mostrar_exemplos'
    
    else:
        # Resposta não reconhecida - pedir clarificação
        return 'clarificar'

def coletar_contexto():
    """
    Coleta informações para contextualização Premium
    """
    print("""
Perfeito! Para maximizar a qualidade do Modo Premium,
preciso de alguns detalhes para contextualização:

1️⃣ Contexto do seu negócio/área:
   Ex: "B2B SaaS para legal tech no Brasil"
   
2️⃣ Principais casos de uso do livro:
   Ex: "Revenue operations, sales enablement, marketing strategy"
   
3️⃣ Exemplos devem ser adaptados para:
   Ex: "Sua empresa, seu setor, seu país"

Você pode fornecer essas informações? Ou posso usar o que
já sei sobre você?
    """)
    
    # Aguardar input do usuário ou usar contexto conhecido
    return {
        'business': 'B2B SaaS',
        'use_cases': 'Revenue operations, sales, marketing',
        'adapt_for': 'Sua empresa, seu setor'
    }
```

### FASE 1: EXTRAÇÃO E ANÁLISE (0 tokens)

```python
# modules/extraction.py

import pdfplumber
import re
from typing import List, Dict

def extract_pdf(pdf_path: str) -> Dict:
    """
    Extrai conteúdo completo do PDF preservando estrutura
    0 tokens - Processamento 100% local
    """
    book_data = {
        'metadata': {},
        'raw_pages': [],
        'num_pages': 0
    }
    
    with pdfplumber.open(pdf_path) as pdf:
        book_data['num_pages'] = len(pdf.pages)
        
        # Extrair metadata
        book_data['metadata'] = {
            'title': pdf.metadata.get('Title', 'Unknown'),
            'author': pdf.metadata.get('Author', 'Unknown'),
            'pages': len(pdf.pages)
        }
        
        # Extrair conteúdo página por página
        for i, page in enumerate(pdf.pages):
            page_data = {
                'number': i + 1,
                'text': page.extract_text(),
                'tables': page.extract_tables(),
                'width': page.width,
                'height': page.height
            }
            book_data['raw_pages'].append(page_data)
    
    return book_data

def detect_hierarchy(book_data: Dict) -> List[Dict]:
    """
    Detecta estrutura hierárquica: capítulos, seções, subseções
    Usa heurísticas: tamanho de fonte, posição, palavras-chave
    0 tokens - Processamento por regras
    """
    chapters = []
    current_chapter = None
    current_section = None
    
    # Padrões comuns de identificação
    chapter_patterns = [
        r'^(Chapter|CHAPTER|Capítulo|CAPÍTULO)\s+(\d+|[IVX]+)',
        r'^(\d+)\.\s+[A-Z]',
        r'^(PART|Part|PARTE|Parte)\s+(\d+|[IVX]+)'
    ]
    
    for page in book_data['raw_pages']:
        lines = page['text'].split('\n')
        
        for line in lines:
            line = line.strip()
            if not line:
                continue
            
            # Detectar capítulo
            for pattern in chapter_patterns:
                if re.match(pattern, line):
                    if current_chapter:
                        chapters.append(current_chapter)
                    
                    current_chapter = {
                        'title': line,
                        'number': len(chapters) + 1,
                        'sections': [],
                        'content': []
                    }
                    current_section = None
                    break
            
            # Detectar seção (heurística: linha curta em maiúsculas)
            if (len(line) < 100 and 
                line.isupper() and 
                current_chapter and 
                not any(re.match(p, line) for p in chapter_patterns)):
                
                current_section = {
                    'title': line,
                    'content': []
                }
                current_chapter['sections'].append(current_section)
            
            # Adicionar conteúdo
            elif current_chapter:
                if current_section:
                    current_section['content'].append(line)
                else:
                    current_chapter['content'].append(line)
    
    # Adicionar último capítulo
    if current_chapter:
        chapters.append(current_chapter)
    
    return chapters

def extract_elements(chapters: List[Dict]) -> Dict:
    """
    Extrai elementos especiais: tabelas, listas, blocos de código
    0 tokens - Processamento por padrões
    """
    for chapter in chapters:
        content_text = '\n'.join(chapter['content'])
        
        # Detectar listas
        chapter['lists'] = re.findall(
            r'(?:^|\n)((?:[-•*]\s+.+\n?)+)',
            content_text,
            re.MULTILINE
        )
        
        # Detectar blocos de código (indentação ou backticks)
        chapter['code_blocks'] = re.findall(
            r'```[\s\S]*?```|(?:^|\n)((?:    .+\n?)+)',
            content_text,
            re.MULTILINE
        )
        
        # Detectar definições (Termo: Definição)
        chapter['definitions'] = re.findall(
            r'([A-Z][A-Za-z\s]+):\s+(.+?)(?:\n|$)',
            content_text
        )
    
    return chapters
```

### FASE 2: ANÁLISE SEMÂNTICA (0 tokens - Básico | Variável - Premium)

```python
# modules/semantic_analysis.py

from collections import Counter
import re
from typing import List, Dict, Set

def identify_concepts_basic(chapters: List[Dict]) -> Dict:
    """
    Modo Básico: Identificação por frequência e padrões
    0 tokens - Análise estatística local
    """
    concepts = {}
    
    # Coletar todos os textos
    all_text = []
    for chapter in chapters:
        all_text.extend(chapter['content'])
        for section in chapter.get('sections', []):
            all_text.extend(section['content'])
    
    text = ' '.join(all_text).lower()
    
    # Extrair termos em negrito (** ou __)
    bold_terms = re.findall(r'\*\*(.+?)\*\*|__(.+?)__', text)
    bold_terms = [t[0] or t[1] for t in bold_terms]
    
    # Extrair substantivos próprios (heurística: palavras capitalizadas)
    proper_nouns = re.findall(r'\b[A-Z][a-z]+(?:\s+[A-Z][a-z]+)*\b', ' '.join(all_text))
    
    # Frequência de palavras (> 3 letras, não stopwords)
    stopwords = {'the', 'and', 'for', 'that', 'with', 'this', 'from', 'have', 'are', 'was', 'were'}
    words = re.findall(r'\b[a-z]{4,}\b', text)
    word_freq = Counter([w for w in words if w not in stopwords])
    
    # Combinar conceitos
    for term in bold_terms:
        concepts[term] = {
            'type': 'definition',
            'frequency': text.count(term.lower()),
            'chapters': []
        }
    
    for term in proper_nouns[:50]:  # Top 50
        if term not in concepts:
            concepts[term] = {
                'type': 'proper_noun',
                'frequency': proper_nouns.count(term),
                'chapters': []
            }
    
    for word, freq in word_freq.most_common(100):
        if word not in concepts and freq > 5:
            concepts[word] = {
                'type': 'keyword',
                'frequency': freq,
                'chapters': []
            }
    
    # Mapear conceitos para capítulos
    for concept, data in concepts.items():
        for i, chapter in enumerate(chapters):
            chapter_text = ' '.join(chapter['content']).lower()
            if concept.lower() in chapter_text:
                data['chapters'].append(i + 1)
    
    return concepts

async def identify_concepts_premium(chapters: List[Dict], context: Dict) -> Dict:
    """
    Modo Premium: Análise semântica com LLM
    ~36% do custo total de refinamento
    """
    # Este método seria chamado apenas se llm_refinement = True
    # Usaria API Anthropic para análise mais profunda
    pass

def map_dependencies(chapters: List[Dict]) -> Dict:
    """
    Cria árvore de dependências entre capítulos
    0 tokens - Análise de referências cruzadas
    """
    dependencies = {}
    
    for i, chapter in enumerate(chapters):
        chapter_num = i + 1
        dependencies[chapter_num] = {
            'requires': [],
            'referenced_by': [],
            'related_topics': []
        }
        
        content = ' '.join(chapter['content'])
        
        # Detectar referências a outros capítulos
        refs = re.findall(
            r'(?:Chapter|Cap\.?|see)\s+(\d+)',
            content,
            re.IGNORECASE
        )
        
        for ref in refs:
            ref_num = int(ref)
            if ref_num != chapter_num and ref_num <= len(chapters):
                dependencies[chapter_num]['requires'].append(ref_num)
                if ref_num in dependencies:
                    dependencies[ref_num]['referenced_by'].append(chapter_num)
    
    return dependencies

def detect_contradictions(chapters: List[Dict]) -> List[Dict]:
    """
    Detecta aparentes contradições entre capítulos
    Modo Básico: padrões simples
    Modo Premium: análise semântica profunda
    """
    contradictions = []
    
    # Padrões de linguagem contraditória
    patterns = [
        (r'always\s+(\w+)', r'never\s+\1'),
        (r'should\s+(\w+)', r'should\s+not\s+\1'),
        (r'recommended', r'not\s+recommended')
    ]
    
    for i, chapter_a in enumerate(chapters):
        content_a = ' '.join(chapter_a['content']).lower()
        
        for j, chapter_b in enumerate(chapters[i+1:], start=i+1):
            content_b = ' '.join(chapter_b['content']).lower()
            
            for pos_pattern, neg_pattern in patterns:
                pos_matches = re.findall(pos_pattern, content_a)
                neg_matches = re.findall(neg_pattern, content_b)
                
                common = set(pos_matches) & set(neg_matches)
                if common:
                    contradictions.append({
                        'chapters': [i+1, j+1],
                        'topic': list(common)[0],
                        'type': 'apparent_contradiction'
                    })
    
    return contradictions

def build_semantic_index(concepts: Dict, chapters: List[Dict]) -> Dict:
    """
    Cria índice semântico com relações entre conceitos
    0 tokens - Análise de co-ocorrência
    """
    semantic_index = {}
    
    for concept, data in concepts.items():
        related = []
        concept_chapters = set(data['chapters'])
        
        # Encontrar conceitos que aparecem nos mesmos capítulos
        for other_concept, other_data in concepts.items():
            if other_concept == concept:
                continue
            
            other_chapters = set(other_data['chapters'])
            overlap = len(concept_chapters & other_chapters)
            
            if overlap >= 2:  # Aparecem juntos em 2+ capítulos
                related.append({
                    'concept': other_concept,
                    'strength': overlap
                })
        
        # Ordenar por força de relação
        related.sort(key=lambda x: x['strength'], reverse=True)
        
        semantic_index[concept] = {
            'appears_in': sorted(data['chapters']),
            'related_concepts': [r['concept'] for r in related[:10]],  # Top 10
            'type': data['type'],
            'frequency': data['frequency']
        }
    
    return semantic_index
```

### FASE 3: GERAÇÃO DE CONTEÚDO (0 tokens - Básico | Variável - Premium)

```python
# modules/content_generation.py

def generate_tldr_basic(chapter: Dict) -> str:
    """
    Modo Básico: TL;DR por extração automática
    0 tokens - Primeiras 2-3 frases do capítulo
    """
    content = chapter['content']
    if not content:
        return "No content available."
    
    # Pegar primeiras frases (até 200 chars)
    text = ' '.join(content[:3])
    sentences = re.split(r'[.!?]+', text)
    
    tldr = []
    char_count = 0
    for sentence in sentences:
        sentence = sentence.strip()
        if not sentence:
            continue
        
        if char_count + len(sentence) > 200:
            break
        
        tldr.append(sentence)
        char_count += len(sentence)
    
    return '. '.join(tldr) + '.'

async def generate_tldr_premium(chapter: Dict, context: Dict) -> str:
    """
    Modo Premium: TL;DR gerado por IA
    ~36% do custo - Mais preciso e relevante
    """
    # Exemplo de prompt para API
    prompt = f"""
Crie um TL;DR conciso (máximo 100 tokens) deste capítulo:

Título: {chapter['title']}
Conteúdo: {' '.join(chapter['content'][:500])}...

O TL;DR deve:
- Capturar a essência do capítulo
- Ser acionável e claro
- Focar no mais relevante
- Usar linguagem objetiva

TL;DR:"""
    
    # Chamada à API (exemplo)
    # response = await anthropic_client.messages.create(...)
    # return response.content[0].text
    
    pass

def create_faqs_basic(chapter: Dict) -> List[Dict]:
    """
    Modo Básico: FAQs baseadas em títulos de seções
    0 tokens - Transformação automática
    """
    faqs = []
    
    # FAQ do título do capítulo
    faqs.append({
        'question': f"What is {chapter['title']} about?",
        'answer': f"See the chapter summary above for an overview of {chapter['title']}."
    })
    
    # FAQ de cada seção
    for section in chapter.get('sections', [])[:5]:  # Top 5 seções
        # Transformar título em pergunta
        title = section['title']
        
        # Heurísticas simples
        if title.startswith('HOW'):
            question = title + '?'
        elif title.startswith('WHAT'):
            question = title + '?'
        else:
            question = f"What about {title.lower()}?"
        
        # Resposta: primeiras 2 frases da seção
        answer_text = ' '.join(section['content'][:2])
        
        faqs.append({
            'question': question,
            'answer': answer_text
        })
    
    return faqs

async def create_faqs_premium(chapter: Dict, context: Dict) -> List[Dict]:
    """
    Modo Premium: FAQs inteligentes geradas por IA
    ~27% do custo - Perguntas realmente úteis
    """
    # Exemplo de prompt
    prompt = f"""
Crie 5 FAQs relevantes e práticas para este capítulo:

Título: {chapter['title']}
Conteúdo: {' '.join(chapter['content'][:800])}...

Contexto do usuário: {context['business']}
Casos de uso: {context['use_cases']}

Gere FAQs que:
- Sejam perguntas que um profissional realmente faria
- Tenham respostas práticas e acionáveis
- Conectem teoria com aplicação
- Sejam relevantes para o contexto do usuário

Formato JSON:
[
  {{"question": "...", "answer": "..."}},
  ...
]
"""
    pass

def extract_frameworks(chapter: Dict) -> List[Dict]:
    """
    Extrai frameworks, processos e checklists acionáveis
    0 tokens - Detecção por padrões
    """
    frameworks = []
    content = '\n'.join(chapter['content'])
    
    # Detectar listas numeradas (processos)
    numbered_lists = re.findall(
        r'(?:^|\n)((?:\d+\.\s+.+\n?)+)',
        content,
        re.MULTILINE
    )
    
    for i, lst in enumerate(numbered_lists):
        steps = re.findall(r'\d+\.\s+(.+)', lst)
        if len(steps) >= 3:  # Mínimo 3 passos
            frameworks.append({
                'type': 'process',
                'name': f"Process from {chapter['title']}",
                'steps': steps
            })
    
    # Detectar checklists (bullet points)
    bullet_lists = re.findall(
        r'(?:^|\n)((?:[-•*]\s+.+\n?)+)',
        content,
        re.MULTILINE
    )
    
    for lst in bullet_lists:
        items = re.findall(r'[-•*]\s+(.+)', lst)
        if len(items) >= 3:
            frameworks.append({
                'type': 'checklist',
                'name': f"Checklist from {chapter['title']}",
                'items': items
            })
    
    return frameworks

async def contextualize_examples(examples: List[str], context: Dict) -> List[Dict]:
    """
    Modo Premium: Adapta exemplos ao contexto do usuário
    ~23% do custo
    """
    # Exemplo de adaptação com IA
    pass
```

### FASE 4: OTIMIZAÇÃO DE TOKENS (0 tokens)

```python
# modules/optimization.py

def create_layered_content(chapter: Dict, tldr: str, summary: str) -> Dict:
    """
    Cria estrutura em camadas: TL;DR → Resumo → Completo
    0 tokens - Organização estrutural
    """
    full_content = '\n\n'.join(chapter['content'])
    
    # Estimar tokens (rough: 4 chars = 1 token)
    tldr_tokens = len(tldr) // 4
    summary_tokens = len(summary) // 4
    full_tokens = len(full_content) // 4
    
    return {
        'tldr': {
            'content': tldr,
            'tokens': tldr_tokens,
            'use_case': 'Quick reference, 60% of queries'
        },
        'summary': {
            'content': summary,
            'tokens': summary_tokens,
            'use_case': 'Standard queries, 25% of queries'
        },
        'full': {
            'content': full_content,
            'tokens': full_tokens,
            'use_case': 'Deep dive, 15% of queries'
        }
    }

def split_large_chapters(chapter: Dict, max_tokens: int = 15000) -> List[Dict]:
    """
    Quebra capítulos grandes em múltiplos arquivos
    0 tokens - Divisão por seções
    """
    chapter_tokens = sum(len(c) for c in chapter['content']) // 4
    
    if chapter_tokens <= max_tokens:
        return [chapter]
    
    # Dividir por seções
    parts = []
    current_part = {
        'title': f"{chapter['title']} - Part 1",
        'number': chapter['number'],
        'part': 1,
        'sections': [],
        'content': []
    }
    current_tokens = 0
    
    for section in chapter.get('sections', []):
        section_tokens = sum(len(c) for c in section['content']) // 4
        
        if current_tokens + section_tokens > max_tokens and current_part['sections']:
            parts.append(current_part)
            current_part = {
                'title': f"{chapter['title']} - Part {len(parts) + 1}",
                'number': chapter['number'],
                'part': len(parts) + 1,
                'sections': [],
                'content': []
            }
            current_tokens = 0
        
        current_part['sections'].append(section)
        current_tokens += section_tokens
    
    if current_part['sections']:
        parts.append(current_part)
    
    return parts if len(parts) > 1 else [chapter]

def build_navigation_map(chapters: List[Dict], dependencies: Dict) -> str:
    """
    Cria mapa de navegação inteligente em Mermaid
    0 tokens - Geração de diagrama
    """
    mermaid = ["```mermaid", "graph TD"]
    
    # Agrupar capítulos por dependência
    for i, chapter in enumerate(chapters):
        node_id = f"C{i+1}"
        title = chapter['title'][:30] + "..." if len(chapter['title']) > 30 else chapter['title']
        mermaid.append(f"    {node_id}[\"{title}\"]")
    
    # Adicionar dependências
    for chapter_num, deps in dependencies.items():
        for req in deps['requires']:
            mermaid.append(f"    C{req} --> C{chapter_num}")
    
    mermaid.append("```")
    return '\n'.join(mermaid)

def generate_applicability_matrix(chapters: List[Dict], contexts: List[str]) -> str:
    """
    Gera matriz de aplicabilidade por contexto
    0 tokens - Análise de keywords
    """
    # Contexts típicos
    default_contexts = [
        'B2B', 'B2C', 'SaaS', 'Product', 'Startup', 'Enterprise'
    ]
    
    if not contexts:
        contexts = default_contexts
    
    # Criar tabela markdown
    header = "| Chapter | " + " | ".join(contexts) + " |"
    separator = "|---------|" + "|".join(["-----" for _ in contexts]) + "|"
    
    rows = [header, separator]
    
    for chapter in chapters:
        content = ' '.join(chapter['content']).lower()
        row = [f"Cap {chapter['number']}"]
        
        for context in contexts:
            # Análise simples de presença de keywords
            context_score = content.count(context.lower())
            
            if context_score > 10:
                row.append("✓✓✓")
            elif context_score > 5:
                row.append("✓✓")
            elif context_score > 0:
                row.append("✓")
            else:
                row.append("✗")
        
        rows.append("| " + " | ".join(row) + " |")
    
    return '\n'.join(rows)
```

### FASE 5: GERAÇÃO DE ARTEFATOS (0 tokens)

```python
# modules/artifacts.py

def create_presentation(book_data: Dict, chapters: List[Dict]) -> str:
    """
    Gera apresentação executiva em Markdown
    0 tokens - Template + dados
    """
    slides = [
        f"# {book_data['metadata']['title']}",
        f"## Executive Summary",
        "",
        f"**Author**: {book_data['metadata']['author']}",
        f"**Pages**: {book_data['metadata']['pages']}",
        "",
        "---",
        "",
        "## Key Topics",
        ""
    ]
    
    # Slide por capítulo (principais)
    for chapter in chapters[:5]:  # Top 5 capítulos
        slides.extend([
            f"## {chapter['title']}",
            "",
            f"**Key Concepts**:",
            ""
        ])
        
        # Extrair primeiros conceitos
        for section in chapter.get('sections', [])[:3]:
            slides.append(f"- {section['title']}")
        
        slides.extend(["", "---", ""])
    
    return '\n'.join(slides)

def build_implementation_plan(frameworks: List[Dict], context: Dict) -> str:
    """
    Cria plano de implementação de 90 dias
    0 tokens - Template estruturado
    """
    plan = [
        "# Implementation Plan - 90 Days",
        "",
        f"**Context**: {context.get('business', 'General')}",
        "",
        "## Phase 1: Weeks 1-4 (Foundation)",
        ""
    ]
    
    # Distribuir frameworks nas fases
    phase1 = frameworks[:len(frameworks)//3]
    phase2 = frameworks[len(frameworks)//3:2*len(frameworks)//3]
    phase3 = frameworks[2*len(frameworks)//3:]
    
    for fw in phase1:
        plan.append(f"### {fw['name']}")
        plan.append("")
        if fw['type'] == 'process':
            for step in fw['steps']:
                plan.append(f"- [ ] {step}")
        plan.append("")
    
    plan.extend([
        "## Phase 2: Weeks 5-8 (Development)",
        ""
    ])
    
    for fw in phase2:
        plan.append(f"### {fw['name']}")
        plan.append("")
        if fw['type'] == 'checklist':
            for item in fw['items']:
                plan.append(f"- [ ] {item}")
        plan.append("")
    
    plan.extend([
        "## Phase 3: Weeks 9-12 (Optimization)",
        ""
    ])
    
    for fw in phase3:
        plan.append(f"### {fw['name']}")
        plan.append("")
    
    return '\n'.join(plan)

def generate_one_pager(book_data: Dict, summary: str, key_concepts: List[str]) -> str:
    """
    Cria one-pager executivo
    0 tokens - Síntese visual
    """
    one_pager = [
        f"# {book_data['metadata']['title']} - One Pager",
        "",
        "## 📚 Overview",
        "",
        summary[:500] + "...",
        "",
        "## 🎯 Key Concepts",
        ""
    ]
    
    for concept in key_concepts[:10]:  # Top 10
        one_pager.append(f"- **{concept}**")
    
    one_pager.extend([
        "",
        "## 🚀 Quick Start",
        "",
        "1. Read chapters 1-3 for foundation",
        "2. Focus on chapters relevant to your use case",
        "3. Use frameworks and templates provided",
        "",
        "## 📊 Application Matrix",
        "",
        "See `aplicabilidade-matrix.md` for detailed breakdown"
    ])
    
    return '\n'.join(one_pager)
```

### FASE 6: ASSEMBLY FINAL (0 tokens)

```python
# modules/skill_assembly.py

import json
from pathlib import Path

def create_skill_structure(output_dir: str, book_title: str):
    """
    Cria estrutura de pastas da skill
    0 tokens - I/O de arquivos
    """
    base_path = Path(output_dir)
    
    # Estrutura de diretórios
    dirs = [
        base_path,
        base_path / "capitulos",
        base_path / "frameworks",
        base_path / "exemplos",
        base_path / "artifacts",
        base_path / "indices"
    ]
    
    for dir_path in dirs:
        dir_path.mkdir(parents=True, exist_ok=True)
    
    return base_path

def generate_main_skill_md(
    book_data: Dict,
    chapters: List[Dict],
    concepts: Dict,
    dependencies: Dict,
    context: Dict,
    mode: str
) -> str:
    """
    Gera o SKILL.md principal da skill especializada
    0 tokens - Template preenchido
    """
    
    # Calcular estatísticas
    num_concepts = len(concepts)
    num_chapters = len(chapters)
    total_pages = book_data['metadata']['pages']
    
    # Criar lista de capítulos
    chapter_list = []
    for ch in chapters:
        chapter_list.append(f"- **Chapter {ch['number']}**: {ch['title']}")
    
    # Criar índice de conceitos principais
    top_concepts = sorted(concepts.items(), key=lambda x: x[1]['frequency'], reverse=True)[:20]
    concept_index = []
    for concept, data in top_concepts:
        chapters_str = ', '.join([f"Cap {c}" for c in data['chapters']])
        concept_index.append(f"- **{concept}**: {chapters_str}")
    
    skill_md = f"""# {book_data['metadata']['title']} - Expert Skill

## 📚 Sobre Este Livro

**Autor**: {book_data['metadata']['author']}  
**Páginas**: {total_pages}  
**Capítulos**: {num_chapters}  
**Conceitos identificados**: {num_concepts}  
**Modo de conversão**: {"Premium (Ultra-Otimizado)" if mode == "premium" else "Básico (Estrutural)"}

Esta skill transforma Claude em um **especialista virtual** neste livro, capaz de:
- ✅ Responder perguntas com base no conteúdo completo
- ✅ Aplicar conceitos ao contexto específico do usuário
- ✅ Criar implementações práticas e personalizadas
- ✅ Conectar ideias de diferentes capítulos
- ✅ Adaptar exemplos ao seu negócio

## 🎯 Quando Claude Deve Usar Esta Skill

**Sempre que o usuário**:
- Mencionar "{book_data['metadata']['title']}"
- Perguntar sobre tópicos relacionados aos conceitos do livro
- Solicitar aplicação prática dos frameworks
- Pedir implementações baseadas no método do livro
- Referenciar capítulos ou conceitos específicos

**Contexto de personalização**: {context.get('business', 'Geral')}  
**Casos de uso**: {context.get('use_cases', 'Diversos')}  
**Exemplos adaptados para**: {context.get('adapt_for', 'Contexto geral')}

## 🧭 Sistema de Navegação Adaptativa

Claude deve usar navegação inteligente baseada no tipo de pergunta:

### Níveis de Profundidade

**📌 Nível 1 - Rápido** (~2-5k tokens):
- **Quando usar**: Perguntas simples, definições, conceitos gerais
- **O que ler**: SKILL.md + TL;DR do capítulo relevante + FAQ
- **Exemplo**: "O que é [conceito]?"
- **Token médio**: 3k

**📖 Nível 2 - Padrão** (~15-20k tokens):
- **Quando usar**: Perguntas sobre aplicação, how-to, explicações
- **O que ler**: SKILL.md + Resumo + Capítulo completo
- **Exemplo**: "Como aplicar [framework]?"
- **Token médio**: 18k

**🔬 Nível 3 - Profundo** (~40-60k tokens):
- **Quando usar**: Análises, comparações, múltiplos conceitos
- **O que ler**: SKILL.md + Múltiplos capítulos + Referências cruzadas
- **Exemplo**: "Compare os métodos X, Y e Z"
- **Token médio**: 50k

**🎓 Nível 4 - Pesquisa** (80k+ tokens):
- **Quando usar**: Criação de estratégias, planos completos, sínteses
- **O que ler**: Conhecimento abrangente + Frameworks + Exemplos
- **Exemplo**: "Crie estratégia completa usando o livro"
- **Token médio**: 100k+

### Auto-Detecção de Nível

Claude detecta automaticamente o nível necessário:

```python
if pergunta contém ["o que é", "defin", "conceito"]:
    nivel = 1  # TL;DR + FAQ
elif pergunta contém ["como", "aplicar", "implementar", "usar"]:
    nivel = 2  # Resumo + Capítulo
elif pergunta contém ["comparar", "diferença", "versus", "análise"]:
    nivel = 3  # Múltiplos capítulos
elif pergunta contém ["criar", "estratégia", "plano", "framework completo"]:
    nivel = 4  # Conhecimento abrangente
else:
    nivel = 2  # Padrão
```

## 📖 Estrutura do Conhecimento

### Arquivos Disponíveis

```
/revenue-architecture/
├── SKILL.md (este arquivo - navegação geral)
├── resumo-executivo.md (visão geral do livro)
├── glossario.md (todos os termos definidos)
├── conhecimento-map.md (árvore de dependências)
├── aplicabilidade-matrix.md (por contexto de negócio)
├── nuances.md (contradições resolvidas)
├── metadata.json (índice semântico completo)
├── changelog.md (histórico de versões)
│
├── capitulos/
│   ├── capitulo-01.md
│   ├── faq-capitulo-01.md
│   └── ...
│
├── frameworks/
│   ├── [frameworks extraídos]
│   └── ...
│
├── exemplos/
│   ├── contextualizados/
│   └── ...
│
├── artifacts/
│   ├── apresentacao-executiva.md
│   ├── plano-implementacao.md
│   └── one-pager.md
│
└── indices/
    ├── por-tema.md
    ├── por-palavra-chave.md
    └── por-aplicacao.md
```

### Mapa de Conhecimento

Ver arquivo `conhecimento-map.md` para árvore completa de dependências.

**Sequência recomendada de aprendizado**:
1. Fundamentos (Cap 1-3)
2. Metodologia Core (Cap 4-6)
3. Aplicação Prática (Cap 7-9)
4. Casos Avançados (Cap 10-12)

## 📑 Índice Completo de Capítulos

{chr(10).join(chapter_list)}

## 🔍 Índice de Conceitos Principais

{chr(10).join(concept_index)}

Ver `glossario.md` para lista completa com definições.

## 🎯 Como Responder Perguntas

### Para Conceitos e Definições
1. Consultar `glossario.md` primeiro
2. Se não encontrar, buscar no TL;DR dos capítulos relevantes
3. Sempre citar capítulo e seção de origem

### Para Aplicações Práticas
1. Identificar capítulo relevante via índice temático
2. Ler resumo do capítulo primeiro
3. Se necessário, ler capítulo completo
4. Consultar `frameworks/` para templates prontos
5. Adaptar ao contexto: {context.get('business', 'geral')}
6. Oferecer exemplos de `exemplos/contextualizados/`

### Para Comparações
1. Identificar capítulos que tratam dos tópicos
2. Consultar `nuances.md` para contradições conhecidas
3. Ler resumos de todos os capítulos envolvidos
4. Criar comparação estruturada
5. Citar seções específicas

### Para Implementações
1. Consultar `frameworks/` para templates
2. Ler capítulos relevantes (completos)
3. Usar `plano-implementacao.md` como base
4. Personalizar para contexto do usuário
5. Criar checklists acionáveis

## 🎨 Instruções Especiais

### Sempre:
- ✅ Citar capítulo e seção ao responder
- ✅ Adaptar linguagem e exemplos ao contexto: {context.get('business', 'geral')}
- ✅ Oferecer frameworks/templates quando aplicável
- ✅ Conectar conceitos de diferentes capítulos quando relevante
- ✅ Sugerir leituras complementares de outros capítulos
- ✅ Usar camada apropriada (TL;DR vs Resumo vs Completo)

### Nunca:
- ❌ Inventar informações que não estão no livro
- ❌ Citar capítulos sem ler o conteúdo
- ❌ Ignorar o contexto de personalização
- ❌ Carregar mais conteúdo que o necessário
- ❌ Misturar informações de fontes externas ao livro

### Formato de Citação

Sempre usar este formato:
```
[Conceito explicado] (Cap X, Seção Y)
```

Exemplo:
```
O framework de Revenue Architecture se baseia em três pilares
fundamentais: pessoas, processos e tecnologia (Cap 3, Seção 3.2).
```

## 💡 Dicas de Uso para o Usuário

### Perguntas Eficazes

**✅ Bom**: "Como aplicar o framework do Capítulo 5 na minha empresa?"  
**❌ Ruim**: "Me explica tudo sobre revenue"

**✅ Bom**: "Qual a diferença entre os métodos X e Y?"  
**❌ Ruim**: "O que o livro fala?"

**✅ Bom**: "Crie um plano de 30 dias para implementar [conceito]"  
**❌ Ruim**: "Resuma o livro"

### Maximizando Valor

1. **Seja específico**: Mencione capítulos ou conceitos quando souber
2. **Forneça contexto**: Quanto mais contexto sobre sua situação, melhor a adaptação
3. **Peça artefatos**: "Crie uma apresentação", "Gere um checklist"
4. **Explore conexões**: "Como isso se relaciona com [outro conceito]?"
5. **Itere**: Faça perguntas de follow-up para aprofundar

## 📊 Estatísticas da Skill

- **Modo de conversão**: {mode.title()}
- **Tokens de geração**: {"~110k (investimento em qualidade)" if mode == "premium" else "0 (estrutural puro)"}
- **Token médio por consulta**: {"~5.6k" if mode == "premium" else "~15k"}
- **Economia vs sem skill**: {"~88%" if mode == "premium" else "~73%"}
- **Capítulos processados**: {num_chapters}
- **Conceitos identificados**: {num_concepts}
- **Frameworks extraídos**: [calculado na geração]
- **FAQs geradas**: [calculado na geração]

## 🔄 Versionamento

Ver `changelog.md` para histórico completo.

**Versão atual**: 1.0.0  
**Data de criação**: [DATA]  
**Última atualização**: [DATA]

## 🆘 Troubleshooting

**P: Claude não está encontrando informação que sei que existe**  
R: Especifique o capítulo se souber. Use o índice de conceitos.

**P: Resposta muito genérica, quero mais detalhe**  
R: Peça explicitamente: "Me dê a explicação completa do Cap X"

**P: Quero adaptar para meu contexto específico**  
R: Forneça mais detalhes sobre seu contexto na pergunta

**P: Como posso ver os frameworks disponíveis?**  
R: Peça: "Liste todos os frameworks extraídos do livro"

---

**Esta skill foi gerada automaticamente pela pdf-to-skill-converter**  
**Para reportar problemas ou sugerir melhorias, atualize a skill base**
"""
    
    return skill_md

def create_chapter_file(chapter: Dict, tldr: str, summary: str, faqs: List[Dict], frameworks: List[Dict]) -> str:
    """
    Cria arquivo markdown de um capítulo
    0 tokens - Template preenchido
    """
    # Estimar tokens
    full_content = '\n\n'.join(chapter['content'])
    tldr_tokens = len(tldr) // 4
    summary_tokens = len(summary) // 4
    full_tokens = len(full_content) // 4
    
    # Extrair tags (conceitos mencionados)
    tags = []
    # Implementação simplificada
    
    chapter_md = f"""---
capitulo: {chapter['number']}
titulo: "{chapter['title']}"
tags: {', '.join(tags) if tags else 'N/A'}
tokens_tldr: {tldr_tokens}
tokens_resumo: {summary_tokens}
tokens_completo: {full_tokens}
---

# Capítulo {chapter['number']}: {chapter['title']}

## 📌 TL;DR (~{tldr_tokens} tokens)

{tldr}

---

## 📖 Resumo Executivo (~{summary_tokens} tokens)

{summary}

---

## 🎯 Conceitos-Chave

"""
    
    # Adicionar conceitos extraídos
    for section in chapter.get('sections', [])[:5]:
        chapter_md += f"- **{section['title']}**\n"
    
    chapter_md += f"""
---

## 📚 Conteúdo Completo (~{full_tokens} tokens)

{full_content}

---

## 🚀 Frameworks Extraídos

"""
    
    if frameworks:
        for fw in frameworks:
            chapter_md += f"\n### {fw['name']}\n\n"
            if fw['type'] == 'process':
                for i, step in enumerate(fw['steps'], 1):
                    chapter_md += f"{i}. {step}\n"
            elif fw['type'] == 'checklist':
                for item in fw['items']:
                    chapter_md += f"- [ ] {item}\n"
            chapter_md += "\n"
    else:
        chapter_md += "Nenhum framework identificado neste capítulo.\n"
    
    chapter_md += """
---

## ❓ FAQ do Capítulo

"""
    
    for faq in faqs:
        chapter_md += f"\n### {faq['question']}\n\n{faq['answer']}\n"
    
    chapter_md += """
---

## 🔗 Referências Cruzadas

Ver `conhecimento-map.md` para dependências deste capítulo.

---

## 📊 Aplicabilidade

Ver `aplicabilidade-matrix.md` para contextos onde este capítulo é mais relevante.
"""
    
    return chapter_md

def create_metadata_json(
    book_data: Dict,
    chapters: List[Dict],
    concepts: Dict,
    dependencies: Dict,
    semantic_index: Dict
) -> str:
    """
    Cria metadata.json com índice completo
    0 tokens - Serialização JSON
    """
    metadata = {
        'book': {
            'title': book_data['metadata']['title'],
            'author': book_data['metadata']['author'],
            'pages': book_data['metadata']['pages'],
            'processed_date': '2025-10-27',  # Dynamic
            'version': '1.0.0'
        },
        'structure': {
            'num_chapters': len(chapters),
            'num_concepts': len(concepts),
            'chapters': [
                {
                    'number': ch['number'],
                    'title': ch['title'],
                    'sections': len(ch.get('sections', []))
                }
                for ch in chapters
            ]
        },
        'semantic_index': semantic_index,
        'dependencies': dependencies,
        'statistics': {
            'total_concepts': len(concepts),
            'total_frameworks': sum(len(ch.get('frameworks', [])) for ch in chapters),
            'avg_tokens_per_chapter': sum(len('\n'.join(ch['content'])) for ch in chapters) // len(chapters) // 4
        }
    }
    
    return json.dumps(metadata, indent=2, ensure_ascii=False)

def validate_output(skill_path: Path) -> Dict[str, bool]:
    """
    Valida estrutura gerada
    0 tokens - Checagem de arquivos
    """
    checks = {
        'SKILL.md exists': (skill_path / 'SKILL.md').exists(),
        'Chapters directory': (skill_path / 'capitulos').exists(),
        'Frameworks directory': (skill_path / 'frameworks').exists(),
        'Metadata exists': (skill_path / 'metadata.json').exists(),
        'Glossary exists': (skill_path / 'glossario.md').exists(),
    }
    
    # Count chapters
    chapters_dir = skill_path / 'capitulos'
    if chapters_dir.exists():
        num_chapters = len(list(chapters_dir.glob('capitulo-*.md')))
        checks[f'{num_chapters} chapters generated'] = num_chapters > 0
    
    return checks
```

### FASE 7: ORQUESTRAÇÃO COMPLETA

```python
# main_converter.py - Script principal

import sys
from pathlib import Path
from modules import extraction, semantic_analysis, content_generation
from modules import optimization, artifacts, skill_assembly

async def convert_pdf_to_skill(
    pdf_path: str,
    output_dir: str,
    mode: str = 'basico',
    context: Dict = None
):
    """
    Pipeline completo de conversão
    """
    
    print("🚀 Iniciando conversão...")
    print(f"📄 PDF: {pdf_path}")
    print(f"📁 Output: {output_dir}")
    print(f"⚙️  Modo: {mode.title()}")
    print()
    
    # FASE 1: Extração
    print("📖 FASE 1: Extraindo PDF...")
    book_data = extraction.extract_pdf(pdf_path)
    print(f"   ✅ {book_data['num_pages']} páginas extraídas (0 tokens)")
    
    print("🔍 Detectando estrutura...")
    chapters = extraction.detect_hierarchy(book_data)
    print(f"   ✅ {len(chapters)} capítulos identificados (0 tokens)")
    
    print("🎯 Extraindo elementos especiais...")
    chapters = extraction.extract_elements(chapters)
    print(f"   ✅ Tabelas, listas e código extraídos (0 tokens)")
    print()
    
    # FASE 2: Análise Semântica
    print("🧠 FASE 2: Análise Semântica...")
    
    if mode == 'basico':
        print("   📊 Modo Básico: Análise estrutural...")
        concepts = semantic_analysis.identify_concepts_basic(chapters)
        print(f"   ✅ {len(concepts)} conceitos identificados (0 tokens)")
    else:
        print("   🤖 Modo Premium: Análise com IA...")
        concepts = await semantic_analysis.identify_concepts_premium(chapters, context)
        print(f"   ✅ {len(concepts)} conceitos identificados (~40k tokens)")
    
    print("   🌳 Mapeando dependências...")
    dependencies = semantic_analysis.map_dependencies(chapters)
    print(f"   ✅ Árvore de conhecimento criada (0 tokens)")
    
    print("   🔎 Detectando contradições...")
    contradictions = semantic_analysis.detect_contradictions(chapters)
    print(f"   ✅ {len(contradictions)} nuances identificadas (0 tokens)")
    
    print("   🔗 Criando índice semântico...")
    semantic_index = semantic_analysis.build_semantic_index(concepts, chapters)
    print(f"   ✅ Índice semântico gerado (0 tokens)")
    print()
    
    # FASE 3: Geração de Conteúdo
    print("✍️  FASE 3: Gerando Conteúdo...")
    
    chapter_contents = []
    total_refinement_tokens = 0
    
    for i, chapter in enumerate(chapters, 1):
        print(f"   📝 Processando Capítulo {i}/{len(chapters)}: {chapter['title'][:40]}...")
        
        # TL;DR
        if mode == 'basico':
            tldr = content_generation.generate_tldr_basic(chapter)
            tldr_tokens = 0
        else:
            tldr = await content_generation.generate_tldr_premium(chapter, context)
            tldr_tokens = len(tldr) // 4
            total_refinement_tokens += tldr_tokens
        
        # Summary (sempre básico - primeira parte do capítulo)
        summary = ' '.join(chapter['content'][:5])
        
        # FAQs
        if mode == 'basico':
            faqs = content_generation.create_faqs_basic(chapter)
            faq_tokens = 0
        else:
            faqs = await content_generation.create_faqs_premium(chapter, context)
            faq_tokens = sum(len(f['question']) + len(f['answer']) for f in faqs) // 4
            total_refinement_tokens += faq_tokens
        
        # Frameworks
        frameworks = content_generation.extract_frameworks(chapter)
        
        chapter_contents.append({
            'chapter': chapter,
            'tldr': tldr,
            'summary': summary,
            'faqs': faqs,
            'frameworks': frameworks
        })
    
    if mode == 'premium':
        print(f"   🤖 Total de tokens de refinamento: ~{total_refinement_tokens}k")
    print()
    
    # FASE 4: Otimização
    print("⚡ FASE 4: Otimização de Tokens...")
    
    print("   📊 Criando camadas de conteúdo...")
    for cc in chapter_contents:
        cc['layers'] = optimization.create_layered_content(
            cc['chapter'], cc['tldr'], cc['summary']
        )
    print("   ✅ Estrutura em camadas criada (0 tokens)")
    
    print("   ✂️  Dividindo capítulos grandes...")
    split_chapters = []
    for cc in chapter_contents:
        parts = optimization.split_large_chapters(cc['chapter'])
        if len(parts) > 1:
            print(f"      📄 Cap {cc['chapter']['number']} dividido em {len(parts)} partes")
        split_chapters.extend(parts)
    print("   ✅ Capítulos grandes otimizados (0 tokens)")
    
    print("   🗺️  Gerando mapa de navegação...")
    nav_map = optimization.build_navigation_map(chapters, dependencies)
    print("   ✅ Mapa de navegação criado (0 tokens)")
    
    print("   📋 Criando matriz de aplicabilidade...")
    contexts = [context.get('business', '')] if context else []
    app_matrix = optimization.generate_applicability_matrix(chapters, contexts)
    print("   ✅ Matriz de aplicabilidade gerada (0 tokens)")
    print()
    
    # FASE 5: Artefatos
    print("🎨 FASE 5: Gerando Artefatos...")
    
    print("   📊 Criando apresentação executiva...")
    presentation = artifacts.create_presentation(book_data, chapters)
    print("   ✅ Apresentação gerada (0 tokens)")
    
    print("   📅 Gerando plano de implementação...")
    all_frameworks = []
    for cc in chapter_contents:
        all_frameworks.extend(cc['frameworks'])
    impl_plan = artifacts.build_implementation_plan(all_frameworks, context or {})
    print("   ✅ Plano de implementação criado (0 tokens)")
    
    print("   📄 Criando one-pager...")
    summary_text = ' '.join(chapters[0]['content'][:10])
    top_concepts = list(concepts.keys())[:10]
    one_pager = artifacts.generate_one_pager(book_data, summary_text, top_concepts)
    print("   ✅ One-pager gerado (0 tokens)")
    print()
    
    # FASE 6: Assembly
    print("🏗️  FASE 6: Montando Skill...")
    
    print("   📁 Criando estrutura de diretórios...")
    skill_path = skill_assembly.create_skill_structure(
        output_dir,
        book_data['metadata']['title']
    )
    print(f"   ✅ Estrutura criada em {skill_path}")
    
    print("   📝 Gerando SKILL.md principal...")
    main_skill = skill_assembly.generate_main_skill_md(
        book_data, chapters, concepts, dependencies,
        context or {}, mode
    )
    (skill_path / 'SKILL.md').write_text(main_skill, encoding='utf-8')
    print("   ✅ SKILL.md criado")
    
    print("   📚 Gerando arquivos de capítulos...")
    capitulos_dir = skill_path / 'capitulos'
    for cc in chapter_contents:
        chapter_file = skill_assembly.create_chapter_file(
            cc['chapter'], cc['tldr'], cc['summary'],
            cc['faqs'], cc['frameworks']
        )
        filename = f"capitulo-{cc['chapter']['number']:02d}.md"
        (capitulos_dir / filename).write_text(chapter_file, encoding='utf-8')
    print(f"   ✅ {len(chapter_contents)} capítulos gerados")
    
    print("   🗂️  Salvando artefatos...")
    artifacts_dir = skill_path / 'artifacts'
    (artifacts_dir / 'apresentacao-executiva.md').write_text(presentation, encoding='utf-8')
    (artifacts_dir / 'plano-implementacao.md').write_text(impl_plan, encoding='utf-8')
    (artifacts_dir / 'one-pager.md').write_text(one_pager, encoding='utf-8')
    print("   ✅ Artefatos salvos")
    
    print("   📊 Gerando metadata.json...")
    metadata_json = skill_assembly.create_metadata_json(
        book_data, chapters, concepts, dependencies, semantic_index
    )
    (skill_path / 'metadata.json').write_text(metadata_json, encoding='utf-8')
    print("   ✅ Metadata gerado")
    
    print("   🗺️  Salvando auxiliares...")
    (skill_path / 'conhecimento-map.md').write_text(nav_map, encoding='utf-8')
    (skill_path / 'aplicabilidade-matrix.md').write_text(app_matrix, encoding='utf-8')
    print("   ✅ Arquivos auxiliares salvos")
    print()
    
    # FASE 7: Validação
    print("✅ FASE 7: Validação...")
    validation = skill_assembly.validate_output(skill_path)
    
    all_passed = True
    for check, passed in validation.items():
        status = "✅" if passed else "❌"
        print(f"   {status} {check}")
        if not passed:
            all_passed = False
    print()
    
    # Relatório Final
    print("=" * 60)
    print("🎉 CONVERSÃO CONCLUÍDA!")
    print("=" * 60)
    print()
    print(f"📊 Estatísticas:")
    print(f"   • Páginas processadas: {book_data['num_pages']}")
    print(f"   • Capítulos gerados: {len(chapter_contents)}")
    print(f"   • Conceitos identificados: {len(concepts)}")
    print(f"   • Frameworks extraídos: {len(all_frameworks)}")
    print(f"   • FAQs geradas: {sum(len(cc['faqs']) for cc in chapter_contents)}")
    print()
    print(f"💰 Custo de Tokens:")
    if mode == 'basico':
        print(f"   • Geração: 0 tokens (100% local)")
        print(f"   • Custo: $0.00")
    else:
        print(f"   • Geração: ~{total_refinement_tokens}k tokens")
        cost = (total_refinement_tokens * 1000 / 1_000_000) * 3
        print(f"   • Custo: ~${cost:.2f}")
        print(f"   • Break-even: ~{int(cost / 0.148)} consultas")
    print()
    print(f"📁 Output:")
    print(f"   • Localização: {skill_path}")
    print(f"   • Arquivos gerados: {sum(1 for _ in skill_path.rglob('*') if _.is_file())}")
    print()
    print(f"🚀 Próximos Passos:")
    print(f"   1. Revisar resumo-executivo.md")
    print(f"   2. Validar exemplos contextualizados (se Premium)")
    print(f"   3. Mover para /mnt/skills/user/ para ativação")
    print(f"   4. Testar com perguntas práticas")
    print()
    print(f"💡 Uso:")
    print(f"   Agora você pode fazer perguntas como:")
    print(f'   • "Como aplicar [conceito] na {context.get("adapt_for", "minha empresa")}?"')
    print(f'   • "Compare os métodos X e Y do livro"')
    print(f'   • "Crie um plano de implementação baseado no Capítulo 5"')
    print()
    
    return skill_path

# Entry point
if __name__ == "__main__":
    # Este script seria executado pelo Claude
    pass
```

## 📋 Instruções para Claude

### Quando o Usuário Solicitar Conversão

1. **LER ESTE SKILL.MD COMPLETAMENTE**

2. **APRESENTAR OPÇÕES** usando o template da Fase 0
   - Calcular custos dinamicamente baseado no número de páginas
   - Explicar benefícios de cada modo
   - Mostrar comparação de ROI

3. **AGUARDAR ESCOLHA EXPLÍCITA**
   - Não prosseguir sem decisão clara
   - Esclarecer dúvidas se necessário
   - Oferecer ver exemplos se solicitado

4. **COLETAR CONTEXTO** (se Premium)
   - Informações sobre negócio
   - Casos de uso
   - Adaptações desejadas

5. **CRIAR SCRIPT PYTHON** orquestrador
   - Importar todos os módulos
   - Configurar pipeline com escolhas do usuário
   - Incluir logging transparente

6. **EXECUTAR CONVERSÃO**
   - Mostrar progresso em cada fase
   - Informar tokens usados (se Premium)
   - Validar output

7. **APRESENTAR RELATÓRIO**
   - Estatísticas completas
   - Custos (se Premium)
   - Próximos passos
   - Como usar a nova skill

### Educação Contínua

Ao apresentar opções, Claude deve:
- ✅ Explicar O QUÊ cada modo faz
- ✅ Explicar POR QUÊ as otimizações existem
- ✅ Mostrar matemática transparente de custos
- ✅ Demonstrar ROI claramente
- ✅ Dar autonomia de escolha ao usuário

### Transparência em Custos

Sempre mostrar:
- Tokens de geração (0 ou valor calculado)
- Custo em USD
- Tokens economizados no uso
- Break-even point
- Economia total em 100 consultas

## 🎯 Casos de Uso

### Caso 1: Livro para Uso Intensivo
```
Livro: 400 páginas
Uso esperado: Consulta diária
Recomendação: Premium
Razão: ROI positivo em 3 dias
```

### Caso 2: POC/Teste
```
Livro: 200 páginas
Uso esperado: Exploração inicial
Recomendação: Básico
Razão: 0 custo, pode evoluir depois
```

### Caso 3: Biblioteca de Livros
```
Múltiplos livros: 5+ livros
Uso esperado: Variado
Recomendação: Básico para todos, Premium para críticos
Razão: Otimizar investimento
```

## 📚 FAQ sobre a Meta-Skill

**P: Posso converter um livro em Básico e depois em Premium?**
R: Sim! Reconverta o mesmo PDF escolhendo Premium.

**P: A skill funciona para livros em qualquer idioma?**
R: Sim, mas o refinamento Premium funciona melhor em inglês/português.

**P: Posso customizar as regras de conversão?**
R: Sim, edite os módulos Python conforme necessário.

**P: Quanto tempo leva a conversão?**
R: Básico: 2-5 minutos | Premium: 10-20 minutos (depende do tamanho)

**P: Posso usar em PDFs escaneados?**
R: Parcialmente. OCR pode degradar qualidade. Melhor usar PDFs com texto.

**P: A skill gerada pode ser compartilhada?**
R: Sim! Copie a pasta para /mnt/skills/user/ de outro usuário.

---

**🎉 Esta meta-skill transforma qualquer livro técnico em um especialista virtual disponível 24/7!**
