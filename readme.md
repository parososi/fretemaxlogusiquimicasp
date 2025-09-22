# 🚛 Calculadora de Frete MAXLOG / GUARULHOS-SP - Usiquímica

Uma calculadora web interativa para cotação de fretes da transportadora MAXLOG, desenvolvida especificamente para o uso limitado a Usiquímica do Brasil. A ferramenta automatiza o cálculo de fretes fracionados e lotação com base na tabela oficial da transportadora.

## 📋 Índice

- [Sobre o Projeto](#sobre-o-projeto)
- [Funcionalidades](#funcionalidades)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Como Usar](#como-usar)
- [Estrutura de Cálculo](#estrutura-de-cálculo)
- [Limitações](#limitações)
- [Créditos](#créditos)
- [Licença](#licença)

## 🎯 Sobre o Projeto

Esta calculadora foi desenvolvida para automatizar e padronizar os cálculos de frete da transportadora MAXLOG, eliminando erros manuais e agilizando o processo de cotação. A ferramenta replica exatamente a tabela oficial da transportadora (Agosto 2025) e inclui todas as taxas aplicáveis.

## ✨ Funcionalidades

### 🧮 Cálculo de Frete
- **Carga Fracionada**: Cálculo por produto individual com rateio de taxas
- **Carga Lotação**: Cálculo por veículo completo (Carreta 32t, 25t, Truck 13t)
- **Múltiplos Produtos**: Suporte para cotação de vários produtos simultaneamente
- **Taxas Automáticas**: GRISS, ADV, Pedágio e Despacho calculados automaticamente

### 📊 Visualizações
- **Timeline de Entrega**: Visualização gráfica dos prazos em dias úteis
- **Gráfico de Custos**: Breakdown visual dos componentes do frete
- **Animações**: Números animados estilo "máquina caça-níqueis"
- **Responsivo**: Interface adaptada para desktop e mobile

### 📄 Documentação
- **Metodologia Detalhada**: Explicação passo-a-passo de cada cálculo
- **Exportação PDF**: Cotação completa em PDF profissional
- **Observações Legais**: Alertas sobre possíveis divergências e limitações

### 🎛️ Interface
- **Design Moderno**: Interface limpa e profissional
- **Tooltips Informativos**: Explicações sobre cada campo
- **Validações**: Verificação de dados em tempo real
- **UX Otimizada**: Fluxo intuitivo e eficiente

## 🛠 Tecnologias Utilizadas

- **HTML5**: Estrutura semântica
- **CSS3**: Estilização moderna com animações
- **JavaScript ES6+**: Lógica de negócio e interatividade
- **Chart.js**: Gráficos interativos
- **jsPDF**: Geração de PDFs
- **Responsive Design**: CSS Grid e Flexbox

## 🚀 Como Usar

### 1. Selecionar Tipo de Carga
- **Fracionada**: Para cargas até 32 toneladas
- **Lotação**: Para veículos completos

### 2. Configurar Origem/Destino
- **Origem**: Guarulhos/SP (fixo)
- **Destino**: Selecionar da lista disponível

### 3. Adicionar Produtos (Fracionada)
- Nome do produto ou código
- Peso em kg
- Valor da Nota Fiscal

### 4. Configurar Lotação
- Selecionar modalidade do frete
- Informar valor da NF

### 5. Calcular e Visualizar
- Clique em "Calcular Frete"
- Visualize resultados detalhados
- Exporte PDF se necessário

### Requisitos
- Navegador moderno (Chrome 80+, Firefox 75+, Safari 13+)
- JavaScript habilitado
- Conexão com internet (para CDNs das bibliotecas)

## 📐 Estrutura de Cálculo

### Carga Fracionada
```
Frete Base (até 100kg) + Excedente + Pedágio + GRISS + ADV + Despacho
```

**Componentes:**
- **Frete Base**: R$ 65,90 a R$ 145,90 (conforme destino)
- **Excedente**: R$ 0,45 a R$ 1,10/kg (acima de 100kg)
- **Pedágio**: R$ 3,50 por fração de 100kg
- **GRISS**: 0,25% sobre valor da NF
- **ADV**: 0,5% sobre valor da NF  
- **Despacho**: R$ 25,00 fixo

### Carga Lotação
```
Frete Veículo + GRISS + ADV
```

**Componentes:**
- **Frete Veículo**: R$ 3.990 a R$ 7.550 (conforme destino/veículo)
- **GRISS**: 0,1% sobre valor da NF
- **ADV**: 0,15% sobre valor da NF

## ⚠️ Limitações

### Importante - Possíveis Divergências
Esta calculadora replica a tabela oficial, mas o valor final pode divergir por:

- **Descontos Comerciais**: Clientes regulares podem ter até 10% de desconto
- **Negociações Específicas**: Acordos particulares entre cliente/transportadora
- **ICMS**: Imposto estadual (12% a 18%) **NÃO incluído**
- **Cubagem**: Cargas volumosas (regra 300kg/m³) podem alterar o cálculo
- **Taxas Adicionais**: TDE (R$ 250), Paletização (R$ 55/palete)

### Uso Recomendado
- ✅ Estimativas rápidas e precisas
- ✅ Comparação entre diferentes cenários
- ✅ Documentação de cotações
- ⚠️ Substituição da cotação oficial da transportadora (compare quando nescessário o cálculo oficial que a transportadora realiza.)

## 👨‍💻 Créditos

**Desenvolvido por:** Paulo Roberto S. S. ([@Parososi](https://github.com/parososi))

### Agradecimentos
- **Usiquímica do Brasil**: Por fornecer os requisitos e tabelas oficiais
- **MAXLOG Transportes**: Pela disponibilização da tabela de preços
- **Comunidade Open Source**: Pelas bibliotecas utilizadas

## 📄 Licença

Este projeto está sob a licença CC BY-NC-ND 4.0 (Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International). Veja o arquivo [LICENSE](LICENSE) para mais detalhes.
