# Arquitetura da solução

<span style="color:red">Pré-requisitos: <a href="05-Projeto-interface.md"> Projeto de interface</a></span>

Definição de como o software é estruturado em termos dos componentes que fazem parte da solução e do ambiente de hospedagem da aplicação.


![Sem título-2025-03-12-2331](https://github.com/user-attachments/assets/ad9de3d6-3099-4fc9-9ba3-b005719fbe7b)

## Funcionalidades

Esta seção apresenta as funcionalidades da solução.

##### Funcionalidade 1 - Cadastro e login de usuários

Permite a criação de conta e login de usuarios do site

* **Instruções de acesso:**
  * Abra o site na pagina cadastro e preencha seus dados, ou login com dados ja cadastrados.
  * 
* **Tela da funcionalidade**:

![Captura de tela 2025-06-29 154105](https://github.com/user-attachments/assets/c6dfa90b-f657-459b-ba42-8a0de2da8e9e)

![Captura de tela 2025-06-29 154115](https://github.com/user-attachments/assets/b818c9ab-32eb-437b-9665-769df0fe78c2)

![Captura de tela 2025-06-29 154120](https://github.com/user-attachments/assets/5b5d1eaa-4976-49b0-9c53-f478a3083ff3)


##### Funcionalidade 2 - homepage

Dashboard com perfil, treinos, blog e dietas

  **Instruções de acesso:**
* apos login acessar homepage do site;
* tera disponivel seção de perfil, blog, dietas e perfil de usuario.

* **Tela da funcionalidade**:

![Captura de tela 2025-06-29 154455](https://github.com/user-attachments/assets/2508b3f1-cc16-45c9-9406-5a5256fd609d)


##### Funcionalidade 3 - Sistema de treinos com filtros, favoritos e IMC

pagina de treinos

**Instruções de acesso:**
* apos acessar homepage, clicar no botao "treinos",
* a pagina ira exibir dados cadastrados na funcionalidade 1 (peso,altura, imc,classificação).
* topicos de treinos logo abaixo dos dados acima (pernas, foco na queima, etc)
* treinos gerais com opção de clicar para ver os detalhes do treino, sendo possivel favorita-lo.

* **Tela da funcionalidade**:
![Captura de tela 2025-06-29 154842](https://github.com/user-attachments/assets/d4295b3d-390a-4d28-a225-1471530b4134)

![Captura de tela 2025-06-29 154901](https://github.com/user-attachments/assets/abae6582-b3a4-42d5-9249-2f8fba52ec42)

![Captura de tela 2025-06-29 154907](https://github.com/user-attachments/assets/a71d2b31-4e79-41a9-8fb3-f876cd6ec706)


##### Funcionalidade 4 - Sistema de dietas e receitas saudáveis
Sistema de dietas e receitas saudáveis

**Instruções de acesso:**
* na homepage clicar em dietas
* sera exibido recomendações do dia
* sera exibido abaixo dicas gerais de saúde
* abaixo lista de receitas separadas por categorias, sendo possivel clicar para ver a receita completa.


**Tela da funcionalidade**:
![Captura de tela 2025-06-29 155318](https://github.com/user-attachments/assets/0bc86180-1809-4567-9868-84f9ab57a77d)

![Captura de tela 2025-06-29 155327](https://github.com/user-attachments/assets/a819cf4f-da44-42b4-9f6b-09bd293e3df1)

![Captura de tela 2025-06-29 155332](https://github.com/user-attachments/assets/8a894da4-1f13-4b4f-8848-22941fc40465)

![Captura de tela 2025-06-29 155338](https://github.com/user-attachments/assets/d17b714f-1e3b-477c-b781-6f7720141b3a)



##### Funcionalidade 5 - Blog com notícias e dicas fitness

Blog com notícias e dicas fitness

**Instruções de acesso:**
* na homepage clicar no botao "blog"
* sera exibidoas noticias mais acessadas, sendo possivel clicar e ler ela completa
* divisao das noticias por topicos/categorias
* card com noticias gerais e botão de ler mais/ compartilhar noticia



**Tela da funcionalidade**:
![Captura de tela 2025-06-29 155730](https://github.com/user-attachments/assets/656a06d4-67e7-4462-94d6-934efedb37ee)

![Captura de tela 2025-06-29 155737](https://github.com/user-attachments/assets/9caf2197-380f-4c2d-97a4-09b2eaac8ab8)

![Captura de tela 2025-06-29 155745](https://github.com/user-attachments/assets/29dd5131-376f-4dc2-b7fa-cb9bd4bff433)



##### Funcionalidade 6 - responsividade



**Tela da funcionalidade**:

![Captura de tela 2025-06-29 160022](https://github.com/user-attachments/assets/798ecbe7-6bff-40ce-af0f-e88ec96a80e3)

![Captura de tela 2025-06-29 160027](https://github.com/user-attachments/assets/a58c7a38-5350-4e4d-924e-37543b531c7f)

![Captura de tela 2025-06-29 160036](https://github.com/user-attachments/assets/da5af87a-8dd6-4ff5-907d-f313fbf98b7b)





### Estruturas de dados

Descrição das estruturas de dados utilizadas na solução com exemplos no formato JSON.Info.

##### Estrutura de dados - Contatos

usuarios

```json
   {
         "usuarios": [
          {
            "id": 1,
            "usuario": "admin",
            "senha": "admin123",
            "email": "admin@onfocus.com"
          },
          {
           "nome": "teste",
           "sobrenome": "teste",
           "altura": "1.80",
           "peso": "67",
           "idade": "18",
           "genero": "Masculino",
           "tempo_disponivel": "60 minutos",
           "local_preferencia": "academia",
           "objetivo": "Massa muscular",
           "experiencia_treinos": "intermediario",
           "usuario": "Cauã",
           "senha": "teste123",
           "email": "teste@gmail.com",
           "id": 2
         }
}
  
```

##### Estrutura de dados - noticias 

noticias

```json
  [
  {
    "id": 1,
    "titulo": "HIIT: O Treino que Revolucionou o Mundo Fitness",
    "imagem": "imagens/treino.jpg",
    "imagens_adicionais": [
      "imagens/hiit-1.jpg",
      "imagens/hiit-2.jpg"
    ],
    "data_publicacao": "2024-03-15",
    "autor": "Dr. Carlos Silva",
    "cargo_autor": "Especialista em Fisiologia do Exercício",
    "tempo_leitura": "8 min",
    "tags": ["Prática de Exercícios", "Saúde e Bem-estar", "Treinamento Funcional"],
    "resumo": "Descubra como o treinamento intervalado de alta intensidade pode maximizar seus resultados em menos tempo, combinando exercícios explosivos com períodos estratégicos de recuperação.",
    "conteudo": "O HIIT (High-Intensity Interval Training) é uma metodologia de treino que revolucionou o mundo fitness por sua eficiência e resultados comprovados. Este método alterna períodos curtos (30-60 segundos) de exercício intenso com períodos de recuperação ativa ou passiva.\n\nBenefícios Científicos:\n- Aumento do EPOC (Excesso de Consumo de Oxigênio Pós-Exercício)\n- Melhora significativa da capacidade cardiovascular\n- Queima de gordura mais eficiente\n- Preservação da massa muscular\n\nProtocolo Básico de HIIT:\n1. Aquecimento (5-10 minutos)\n2. 30 segundos de exercício intenso\n3. 30 segundos de recuperação\n4. Repetir por 8-12 ciclos\n5. Resfriamento (5 minutos)\n\nExercícios Recomendados:\n- Burpees\n- Mountain Climbers\n- Jumping Jacks\n- Polichinelos\n- Corrida no lugar\n\nDicas de Segurança:\n- Consulte um profissional antes de iniciar\n- Mantenha a técnica correta\n- Hidrate-se adequadamente\n- Respeite seus limites\n\nEstudos recentes mostram que 20 minutos de HIIT podem ser tão efetivos quanto 1 hora de exercício moderado contínuo. No entanto, é importante adaptar a intensidade ao seu nível de condicionamento.",
    "referencias": [
      {
        "titulo": "Effects of High-Intensity Interval Training on Health and Fitness",
        "autor": "Journal of Sports Medicine",
        "ano": 2023
      }
    ]
 }
]
```

receitas:
```json
{
    "id": 1,
    "nome": "Salada Colorida de Quinoa",
    "imagem": "imagens/prato.jpg",
    "ingredientes": [
      "1 xícara de quinoa",
      "2 xícaras de água",
      "1 cenoura ralada",
      "1/2 pimentão vermelho picado",
      "1/2 pepino picado",
      "1/2 xícara de milho",
      "1/2 xícara de ervilha",
      "Salsinha a gosto",
      "Sal, azeite e limão a gosto"
    ],
    "modo_preparo": [
      "Lave a quinoa e cozinhe na água até secar.",
      "Deixe esfriar e misture com os demais ingredientes.",
      "Tempere com sal, azeite e limão. Sirva gelada."
    ],
    "tempo_preparo": "20 minutos",
    "rendimento": "4 porções",
    "calorias": 180,
    "tags": ["Vegetariana", "Saudável", "Rápida"],
    "descricao": "Uma salada leve, nutritiva e refrescante, perfeita para dias quentes ou como acompanhamento."
  },
```



### Módulos e APIs

Esta seção apresenta os módulos e APIs utilizados na solução.

**Images**:

* Unsplash - [https://unsplash.com/](https://unsplash.com/) 

**Fonts:**

*fontes - https://fonts.googleapis.com

**Scripts:**

- **Frontend:** HTML5, CSS3, JavaScript (ES6+)
- **Design:** Flexbox, Grid, CSS Custom Properties, SVG, Font Awesome
- **Backend:** Node.js, Express, JSON Server (mock API)
- **Persistência:** localStorage (usuário, favoritos, etc.)
- **Outros:** Toast notifications, animações CSS, modais customizados


