# Testes com RestAssured, JUnit e reports com Allure
Este projeto teve como finalidade explorar a framework RestAssured e JUnit. 
Entretanto, como forma de consolidar os conhecimentos dados, foi dado ênfase maior na geração de reports com o Allure Framework. 
### Como acessar os relatórios com Allure:
* Após dar o fork no projeto, com a IDE de sua escolha acesse o pom.xml, neste projeto seguiremos o passo a passo pelo Intellij.
Note que as configurações na build é extremamente necessária, sem isso não será possivel criar os reports.
* Depois no canto superior direito do intellij procure pela aba maven
* Ao clicá-la aparecerá todas as opções do maven
* Clique em maven goal > maven clean 
* Após dar o clean, deverá aparecer no console BUILD SUCCESS
* Depois clique na opção maven goal > maven test para rodar os testes, no caso do projeto aparecerá: 

![maven-test](URL da imagem)

* Depois maven > plugins > Allure > Allure:report para gerar na pasta target a pasta Allure-results
* Com a execução deverá aparecer no console:
```
[INFO] Report generated successfully.
[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------

```
* Para acessar o site do Allure com o report completo em uma interface amigável execute maven >  plugins > allure > allure:serve
* Abrirá automáticamente uma janela com o site devendo conter as seguintes imagens:

![site-Allure-reports](URL da imagem)

![site-Allure-reports](URL da imagem)

