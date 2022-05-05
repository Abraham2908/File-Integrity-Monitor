<h1>File Integrity Monitor (FIM) - Example of file integrity monitoring</h1>



<h2>Descrição</h2>
<b>Script em PowerShell com o objetivo de realizar o monitoramento da integridade de arquivos. Demonstração do pilar da integridade na segurança da informação e possibilidade de por meio de alertas, detectar comprometimento de arquivos, facilitando sua investigação.<br /> <br />Após a execução, é fornecido ao usuário a opção de gerar um novo arquivo de monitoramento ou passar a escutar(monitorar) um existente. A primeira opção, realiza um check na pasta Files e após verificar os arquivos, armazena o caminho do arquivo e gera um hash (com a utilização da função hash SHA 512). A segunda opção, passa a verificar o arquivo em execução continua, reportando mensagens para o usuário de acordo com o que foi realizado.
</b>

<br />
<h3>Principais pontos do projeto:</h3>
<br />

- Desenvolvimento de script PowerShell personalizado, gerando algoritmos de hash com o objetivo de monitorar a integridade de arquivos e pastas.<br /><br />
- Utilização de função hash SHA 512.<br /><br />
- Criação de arquivo txt com caminhos e respectivos hashes de arquivos para possibilitar o monitoramento, em caso de já existir um arquivo com essas informações o script   exclui o existente e cria um novo arquivo para evitar a duplicidade.<br /><br />
- Comparação continua de arquivos/pastas vs baseline, retornando alertas se qualquer mudança for detectada.<br /><br />
- Emite alertas enquanto em execução das alterações relacionadas aos arquivos como: inclusão, exclusão e alteração. Possibilitando uma investigação mais aprofundada do comprometimento<br /><br />
<br />
<br />

<p align="center">
<img src="https://i.imgur.com/DCT60Ll.png" height="85%" width="85%" alt="pws example"/>
</p>
<br />
<p align="center">
<img src="https://i.imgur.com/2kihf5p.png" height="85%" width="85%" alt="pws example 2"/>
</p>
<br />
<p align="center">
<img src="https://i.imgur.com/OaIRrEC.png" height="85%" width="85%" alt="pws example 3"/>
</p>
<br />
<p align="center">
<img src="https://i.imgur.com/ypdHYk5.png" height="85%" width="85%" alt="pws example 4"/>
</p>

<h4>Monitoramento:</h3>
- Vermelho/Cinza: Arquivos deletados.<br /><br />
- Amarelo: Arquivos modificados.<br /><br />
- Verde: Arquivos criados.<br /><br />
<br />
<p align="center">
<img src="https://i.imgur.com/sCXw0nO.png" height="85%" width="85%" alt="PWS example5"/>
</p>
<br />
<h2>Linguagens</h2>

- <b>PowerShell:</b> Script para verificar e monitorar a integridade de arquivos através de função hash (SHA 512)


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
