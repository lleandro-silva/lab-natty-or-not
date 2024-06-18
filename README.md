# Natural ou Fake Natty? Como Vencer na Era das IAs Generativas

## 🚀 Introdução

> Woooow! Look at this 👀

Olá pessoal, Venilton da DIO aqui! Inspirado na hype _"Natty or Not"_ do fisiculturismo, este Lab da DIO te convida a conhecer o mundo das IAs Generativas, explorando o potencial dessas tendências tecnológicas incríveis!

## 🎯 Bora Pro Desafio!? Você Já Venceu 💪🤓

### Objetivos

1. **Explorar IAs Generativas**: Utilize essas tecnologias para criar conteúdos que sejam o mais realista possível. Seja criativo! Você pode produzir imagens, textos, áudios, vídeos ou combinações de tudo isso!
1. **Potfólio de Projetos**:
    1. Faça o "fork" deste repositório, criando uma cópia em seu GitHub pessoal;
    2. Edite seu README com os detalhes do seu projeto, siga nosso [Template](#template) (é só copiar, colar e preencher);
    3. Submeta o link do seu repositório na plataforma da DIO. Pronto, você acabou de fortalecer seu portfólio de projetos nos perfis do GitHub e DIO 🚀
1. **Efeito de Rede**: Compartilhe seus resultados nas redes sociais com a hashtag **#LabDIONattyOrNot**. Não esqueça de nos marcar: [DIO](https://www.linkedin.com/school/dio-makethechange) e [falvojr](https://www.linkedin.com/in/falvojr).

### Template

```markdown
# Explorando a Criatividade com IA Generativa ;)

## 📒 Descrição
Este projeto visa explorar o potencial das Inteligências Artificiais Generativas (IAs Generativas) para criar conteúdos originais e criativos, abrangendo texto, imagem e áudio. Utilizando diversas tecnologias de IA, o objetivo é demonstrar como essas ferramentas podem ser aplicadas para gerar novas formas de expressão e arte digital.

## 🤖 Tecnologias Utilizadas
GPT (Generative Pre-trained Transformer) para geração de texto.
DALL-E para geração de imagens a partir de descrições textuais.
StyleGAN para geração de imagens realistas.
WaveGAN e WaveNet para geração de áudio realista.
Frameworks de aprendizado profundo como TensorFlow ou PyTorch para implementação dos modelos.
Linguagens de programação como Python para desenvolvimento e integração.

## 🧐 Processo de Criação
1. Planejamento e Pesquisa
- Definição dos objetivos do projeto: explorar diferentes tipos de IA Generativas e suas capacidades.
- Pesquisa sobre as tecnologias disponíveis, incluindo GPT, DALL-E, StyleGAN, e outras ferramentas relevantes.
2. Desenvolvimento
- Implementação de modelos de IA Generativas selecionados para cada tipo de conteúdo (texto, imagem, áudio).
- Treinamento ou utilização de modelos pré-treinados, dependendo da complexidade e dos recursos disponíveis.
- Integração das tecnologias em um ambiente de desenvolvimento adequado, garantindo interoperabilidade e eficiência.
3. Experimentação e Iteração
- Geração de amostras de conteúdo utilizando diferentes configurações e parâmetros dos modelos.
- Avaliação da qualidade e originalidade dos resultados gerados.
- Ajustes nos modelos e técnicas conforme necessário para melhorar os resultados.
4. Implementação e Demonstração
- Criação de uma interface ou plataforma para demonstrar os resultados do projeto.
- Integração dos diferentes tipos de conteúdo gerados (texto, imagem, áudio) em um fluxo coerente e interativo.
- Preparação de documentação e materiais educativos para compartilhar aprendizados e técnicas utilizadas.

## 🚀 Resultados
Demonstração de capacidades avançadas de geração de conteúdo através de IA Generativa.
Amostras de texto geradas com coerência e relevância semelhantes ao humano.
Imagens geradas com detalhes e estilos variados, refletindo descrições textuais fornecidas.
Áudio gerado com qualidade próxima à humana, incluindo fala e música.

## 💭 Reflexão (Opcional)
Este projeto destacou não apenas as capacidades impressionantes das IAs Generativas em criar conteúdo novo e original,
mas também os desafios e considerações éticas envolvidas. A flexibilidade e a adaptabilidade dos modelos permitiram
explorar uma variedade de formas de expressão artística e criativa, ao mesmo tempo em que ressaltou a importância de
uma supervisão cuidadosa e crítica durante o processo de desenvolvimento. Além disso, a integração de diferentes
tipos de IA Generativa em um projeto unificado demonstrou o potencial transformador dessas tecnologias no campo da
criação digital e além.

## Codando....

Utilização do GPT-3 para Geração de Texto

import openai

# Define sua chave da API da OpenAI
openai.api_key = 'sua-chave-de-api-aqui'

def gerar_texto_gpt(prompt, max_tokens=150):
    response = openai.Completion.create(
        engine="davinci-codex",  # GPT-4, mais avançado que o GPT-3
        prompt=prompt,
        max_tokens=max_tokens,
        stop=None,
    )
    return response.choices[0].text.strip()

# Exemplo de uso
prompt = "Um poema sobre o pôr do sol"
texto_gerado = gerar_texto_gpt(prompt)
print(texto_gerado)

Utilização do DALL-E para Geração de Imagens

import requests
from PIL import Image
from io import BytesIO

def gerar_imagem_dalle(descricao):
    response = requests.post(
        'https://api.openai.com/v1/images', 
        headers={'Authorization': f'Bearer {openai.api_key}'},
        json={'prompt': descricao}
    )
    url = response.json()['data']['url']
    image = Image.open(BytesIO(requests.get(url).content))
    return image

# Exemplo de uso
descricao = "uma árvore tropical com um céu estrelado ao fundo"
imagem_gerada = gerar_imagem_dalle(descricao)
imagem_gerada.show()
```

### Exemplos e Insigths

- [E-BOOK](/exemplos/E-BOOK.md)
- [Podcast](/exemplos/PODCAST.md)
- [Vídeo (Avatar Virtual)](/exemplos/VIDEO.md)

## Links Interessantes

[Base10: If You’re Not First, You’re Last: How AI Becomes Mission Critical](https://base10.vc/post/generative-ai-mission-critical/)

![Base10's Trend Map Generative AI](https://github.com/digitalinnovationone/lab-natty-or-not/assets/730492/f4df26e8-f8f7-4419-8252-c69d73ea930c)
