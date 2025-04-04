# MIST List Search and Converter

![MIST List Search and Converter](https://i.ibb.co/WgkSgzc/f5f56807-238e-40b8-a6e7-4baf2608d219-1.gif)

## Descrição

MIST List Search and Converter é uma ferramenta web desenvolvida para facilitar a conversão de listas de nomes de veículos entre diferentes formatos utilizados em vários frameworks e scripts para FiveM. A ferramenta permite extrair nomes de modelos de veículos de arquivos `vehicles.meta` ou converter manualmente listas de texto para formatos compatíveis com recursos populares.

## Funcionalidades

- **Extração automática** de nomes de modelos de veículos de arquivos `vehicles.meta`
- **Conversão de listas** para os seguintes formatos:
  - QBCore
  - ec-dealership
  - mist-cars-spawn
  - PDM
  - 0r_vehicleshop
  - lsrp_vehicleshop
- **Tema claro/escuro** para melhor experiência de usuário
- **Interface responsiva** adaptada para dispositivos móveis e desktop
- **Copiar para área de transferência** com um clique

## Como usar

### Método 1: Extração de pasta

1. Clique no botão "Select Folder"
2. Selecione a pasta que contém os arquivos `vehicles.meta` dos veículos
3. A ferramenta extrairá automaticamente os nomes dos modelos
4. Selecione o formato desejado no menu suspenso
5. Clique em "Convert List"
6. Use o botão "Copy Converted List" para copiar o resultado

### Método 2: Entrada manual

1. Cole uma lista de nomes de modelos de veículos na área de texto esquerda
2. Cada nome de modelo deve estar em uma linha separada
3. Selecione o formato desejado no menu suspenso
4. Clique em "Convert List"
5. Use o botão "Copy Converted List" para copiar o resultado

## Formatos de conversão

### QBCore
```lua
['modelName'] = {
    ['name'] = 'Model Name',
    ['brand'] = 'Unknown',
    ['model'] = 'modelName',
    ['price'] = 50000,
    ['category'] = 'unknown',
    ['categoryLabel'] = 'Unknown',
    ['hash'] = `modelName`,
    ['shop'] = 'pdm',
},
```

### ec-dealership
```lua
{
    type = "car",
    model = "modelName",
    label = "MODEL NAME",
    price = 10
},
```

### mist-cars-spawn
```lua
{nome = "Model Name", modelo = "modelName", description = "car"},
```

### PDM
```lua
{
    name = "Model Name", model = "modelName", 
    icon = "bars", iconColor = "#ffffff", 
    price = 100000, description = "This is a description",
    stats = {
        maxspeed = "200",
        acceleration = "3.7",
        braking = "1.9",
        handling = "7",
        steering = "5"
    }
},
```

### 0r_vehicleshop
```lua
{label = "Model Name", model = "modelName", price = 1},
```

### lsrp_vehicleshop
```lua
{label = 'Model Name', VEHICLE_MODEL = joaat('modelName'), VEHICLE_PRICE = 20000},
```

## Tecnologias utilizadas

- HTML5
- CSS3 (incluindo animações e tema claro/escuro)
- JavaScript (ES6+)
- FileReader API para leitura de arquivos

## Instalação

1. Clone o repositório:
```bash
git clone https://github.com/MIST145/mist-list-converter.git
```

2. Abra o arquivo `index.html` em seu navegador

## Uso online

Você também pode acessar a ferramenta online sem necessidade de download.

## Compatibilidade

A ferramenta é compatível com os navegadores modernos:
- Chrome
- Firefox
- Safari
- Edge

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests com melhorias.

1. Faça um fork do projeto
2. Crie sua branch de feature (`git checkout -b feature/nova-funcionalidade`)
3. Commit suas alterações (`git commit -m 'Adiciona nova funcionalidade'`)
4. Push para a branch (`git push origin feature/nova-funcionalidade`)
5. Abra um Pull Request

## Contato

- Discord: mist_goat
- GitHub: [MIST145](https://github.com/MIST145)

## Licença

Este projeto está sob a licença MIT. Consulte o arquivo `LICENSE` para obter mais informações.

## Agradecimentos

- Desenvolvido por MIST
- Ícones e animações por vários criadores

---

**Nota:** Esta ferramenta foi criada para auxiliar desenvolvedores de recursos para FiveM, facilitando a conversão de listas de veículos entre diferentes formatos de scripts.
