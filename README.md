# Testes com RestAssured, JUnit,reports com Allure e teste estático com o uso da ferramenta PMD

Este projeto teve como finalidade explorar a framework RestAssured e JUnit. 
Entretanto, como forma de consolidar os conhecimentos dados, foi dado ênfase maior na geração de reports com o Allure Framework. Também, procurei explorar o conceito dos testes estáticos com o uso do PMD.

### PMD
<img src = "https://github.com/Denise-Melo/Testes-com-RestAssured-JUnit-e-Allure/blob/main/teste-estatico-pmd/pmd.png" width="800px" height= "400px">

### Como criar os relatórios com Allure:
* Após dar o fork no projeto, com a IDE de sua escolha acesse o pom.xml, neste projeto seguiremos o passo a passo pelo Intellij.
  Note que as configurações na build é extremamente necessária, sem isso não será possivel criar os reports.
* Depois no canto superior direito do intellij procure pela aba maven
* Ao clicá-la aparecerá todas as opções do maven
* Clique em maven goal > **maven clean**
* Após dar o clean, deverá aparecer no console BUILD SUCCESS
* Depois clique na opção maven goal > **maven test** para rodar os testes e criar a pasta target, no caso do projeto aparecerá: 

![maven-test](https://github.com/Denise-Melo/testes-RestAssured--JUnit-/blob/main/imagens-allure/imagem-do-console-apos-rodar-maven-test.png)

* Depois maven > plugins > Allure > **Allure:report** para gerar na pasta target a pasta Allure-results
* Com a execução deverá aparecer no console:
```
[INFO] Report generated successfully.
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------

```
* Para acessar o site do Allure com o report completo em uma interface amigável execute maven >  plugins > allure >  e escolha a opção allure:serve
* Abrirá automaticamente uma janela com o site devendo conter as seguintes imagens: (caso essa opçao não dê certo, apresento outra opção ao final das imagens)

##### Tela inicial do Allure com reports
![site-Allure-reports](https://github.com/Denise-Melo/Testes-com-RestAssured-JUnit-e-Allure/blob/main/imagens-allure/tela-inicial-allure-com-os-3-testes.png)

##### Tela do gráfico
![site-Allure-reports](https://github.com/Denise-Melo/Testes-com-RestAssured-JUnit-e-Allure/blob/main/imagens-allure/grafico-allure-report.png)

###
#### Caso a tela não abra automaticamente com o allure:serve, podemos parar de rodar o servidor no terminal clicando no quadrado vermelho e nos direcionar para a pasta target :

* site > index.html > com o botão direito clicar na opção open in > Browser > escolha o de sua preferência
* Caso a pasta site em target não abra, será preciso repetir o processo começando com maven clean, maven test, Allure:report para então conseguir abrir a pasta site;

