[![HitCount](http://hits.dwyl.com/learning-crawlers/Prefeitura-Rio-de-Janeiro-Remuneracao.svg)](http://hits.dwyl.com/learning-crawlers/Prefeitura-Rio-de-Janeiro-Remuneracao)

# Prefeitura do Rio de Janeiro Remuneração
Extração de dados com Selenium + BeautifulSoup para listar pagamentos da Prefeitura do Rio de Janeiro

**Executado com python v3.7**


## Install

Download & Install Browser

### Google Chrome Stable:

**Linux**

```bash
wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
sudo apt install ./google-chrome-stable_current_amd64.deb -y
```

**Windows**

Download page: https://www.google.pt/intl/pt-PT/chrome/

**Next**, download Google Chrome Driver from here: https://chromedriver.chromium.org/downloads
 
### Firefox:

**Linux**

```bash
sudo apt install firefox -y
```

**Windows**

Download page: https://www.mozilla.org/pt-BR/firefox/new/

**Next**, download Google Chrome Driver from here: https://github.com/mozilla/geckodriver/releases

### Tesseract:

Install tesseract using windows installer available at: https://github.com/UB-Mannheim/tesseract/wiki


## City hall of Rio de Janeiro (Public Agencies)

- Agência de Fomento do Município do Rio de Janeiro S.A.
- Companhia Carioca de Securitização
- Companhia Municipal de Conservação e Obras Públicas
- Companhia Municipal de Energia e Iluminação
- Companhia Municipal de Limpeza Urbana
- Companhia de Desenvolvimento Urbano da Região do Porto do Rio de Janeiro
- Companhia de Engenharia de Tráfego do Rio de Janeiro
- Controladoria Geral do Município do Rio de Janeiro
- Distribuidora de Filmes S.A.
- Empresa Municipal de Artes Gráficas S.A.
- Empresa Municipal de Informática S.A.
- Empresa Municipal de Urbanização - RIO-URBE
- Empresa Pública de Saúde do Rio de Janeiro S/A
- Empresa de Turismo do Município do Rio de Janeiro
- Fundação Cidade das Artes
- Fundação Instituto das Águas do Município do Rio de Janeiro
- Fundação Instituto de Geotécnica do Município do Rio de Janeiro
- Fundação Jardim Zoológico da Cidade do Rio de Janeiro
- Fundação Parques e Jardins
- Fundação Planetário da Cidade do Rio de Janeiro
- Gabinete do Prefeito
- Guarda Municipal do Rio de Janeiro
- Instituto Municipal de Urbanismo Pereira Passos
- Instituto de Previdência e Assistência do Município do Rio de Janeiro
- MULTIRIO - Empresa Municipal de Multimeios Ltda.
- Procuradoria Geral do Município do Rio de Janeiro
- Riocentro S.A. - Centro de Feiras, Exposições e Congressos do Rio de Janeiro
- Secretaria Especial de Turismo
- Secretaria Municipal da Casa Civil
- Secretaria Municipal da Pessoa com Deficiência e Tecnologia
- Secretaria Municipal de Assistência Social e Direitos Humanos
- Secretaria Municipal de Cultura
- Secretaria Municipal de Desenvolvimento, Emprego e Inovação
- Secretaria Municipal de Educação
- Secretaria Municipal de Fazenda
- Secretaria Municipal de Infraestrutura, Habitação e Conservação
- Secretaria Municipal de Meio Ambiente da Cidade
- Secretaria Municipal de Ordem Pública
- Secretaria Municipal de Saúde
- Secretaria Municipal de Transportes
- Secretaria Municipal de Urbanismo
- Secretaria Municipal do Envelhecimento Saudável, Qualidade de Vida e Eventos


## Running

Execute run.py file:

```bash
python run.py
```


## Result

**Schema**

- date_scraping: string
- url: string
- orgao: string
- matricula: string
- nome: string
- lotacao: string
- mes_ano: string
- folha: string
- vantagens: string
- descontos: string
- liquido: string

**Data**

```json
{
    "date_scraping": "2020-02-24 03:20:21",
    "url": "http://jeap.rio.rj.gov.br/contrachequeapi/transparencia",
    "orgao": "Secretaria Municipal de Urbanismo",
    "matricula": "1451426",
    "nome": "ANTONIO LUIZ BARBOZA CORREIA",
    "lotacao": "SMU",
    "mes_ano": "01/2020",
    "folha": "NORMAL",
    "vantagens": "32.967,34",
    "descontos": "9.021,26",
    "liquido": "23.946,08"
}
```

Please, if you find a bug feel free to contribute!