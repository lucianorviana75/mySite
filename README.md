
# mySite

<!DOCTYPE html>
<html lang="pt">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Tecnologic_LRV</title>
        <link rel="stylesheet" href="mySite.css">
    </head>
    <body>
        <h4 style="color: #7bac3b; border-bottom: 1px solid #7bac3b; margin-top: 0px; margin-bottom: 10px; font-family: Lato">Tópicos</h4>
        <div style="line-height: 24px"><a style="font-family: Lato; color: #3f403d; font-size: 14px" href="#Fase analise" title="Fase analise">Fase de analise</a></div>
        
        <div style="line-height: 24px"><a style="font-family: Lato; color: #3f403d; font-size: 14px" href="#Fase da modelagem;" title="Fase da modelagem">Fase da modelagem</a></div>
        <div style="line-height: 24px"><a style="font-family: Lato; color: #3f403d; font-size: 14px" href="#sintaxe" title="Sintaxe">Sintaxe</a></div>
        
        <h1>Logica de programação</h1>
        <h2>A análise e a síntese de um problema</h2>
        

        <div>
           
                <h3>Existem duas grandes fases na resolução de um problema ,a análise e síntese. </h3>
            
            <p>
                <h3 id="Fase analise">Fase da análise = O problema é entendido de forma,que se descubra o que deve ser solucionado.</h3>
                <b>
                    # [1] Quais são os dados necessários.
                    # [2] Quais são as condições necessárias para resolvê-lo.
                    # [3] Se são insuficientes ou redundantes, ou ainda contraditórios.
                    Então parte-se para a modelagem.
                </b>
            </p>
            <p>
                <h3 id="Fase da modelagem;">Fase da modelagem;</h3>
                <b>
                    # Pode ser enriquecidos com o auxilio de equações desenhos ou gráficos.
                    # Como resultado dessa fase , se tem a elaboração de um plano de ação, no qual pode se ter uso de problemas auxiliares.
                    # O uso direto de abstração, o que significa elaborar modelos mentais do problema em questão ,
                    e do encaminhamento de sua solução.
                </b>
            </p>
            <p>
                <h3 id="sintaxe">Síntese;</h3>
                <b># Executa-se o plano definido na fase de analise, representado os passos por meio de algoritmo.<br># Usaremos como exemplo a torre de Hanoi.</b></h3>
                
            </p>
        </div>    
        <div>
            <pre><code class="modelo" contentEditable="true"> 
            <H3>Algoritmo</H3>
               <b>INICIO</b>
                    #1° - Repita [repetir a execução das duas linhas abaixo até que a condição na parte até seja atendida].
                    #2° - Mova o menor anel de sua haste atual para a próxima no sentido horário.
                    #3° - Execute o único movimento possível com um anel que não seja o menor de todos.
                    #4° - Até que todos os discos tenham sido transferidos para outra haste.
               <b>FIM</b> 
            </code></pre>    
        </div>
         
        <div>
            <pre><code class="formula" contentEditable="true"> 
                <h3>Codigo Python</h3>   
                print(
                '''
                TORRE DE HANOI
                [1]-Mover um anel da haste A para a haste B.
                [2]-Mover um anel da haste A para a haste C.
                [3]-Mover um anel da haste B para a haste C.
                [4]-Mover um anel da haste A para a haste B.
                [5]-Mover um anel da haste C para a haste A.
                [6]-Mover um anel da haste C para a haste B.
                [7]-Mover um anel da haste A para a haste B.
                
                Situação, três hastes A,B,C ,na haste A repousam três anéis de diâmetro diferentes,
                o objetivo é terminar com os três anéis na haste B ,o anél maior vem primeiro de baixo pra
                cima fechando com o menor em cima.
                
                O objetivo é transferir os três anéis da haste A para B, usando C se necessário.As regras de movimento são :
                [1] deve-se mover um único anel por vez.
                [2] um anel de diâmetro maior nunca pode repousar sobre algum outro de diâmetro menor.
                '''
                )
                print('-'* 80)
                print('''
                    [1] Anél maior.
                    [2] Anél medio.
                    [3] Anel menor.
                    [-]
                    [4] primeira haste
                    [5] segunda haste
                    [6] terceira haste
                ''')
                print('-'* 80)
                while True:
                    Anel = int(input("Escolha um anél ,[1]=maior,[2]=media ou [3]=menor, para movimentar . "))
                    print(f"Você escolheu o anél n°[{Anel}]")
                    if Anel < 1  :
                        print("Este anel nao existe")
                        print("de novo")
                        break
                    elif Anel > 3:
                        print("Este anel não existe")
                        print("de novo")
                        break
                    haste = int(input("Escolha uma haste ,[4]=primeira haste,[5]=segunda haste ou [6]=terceira haste. "))
                    print(f'Você escolheu haste n°[{haste}]')
                    if haste < 4:
                        print("Esta haste não existe")
                        print("De novo")
                        break
                    elif haste > 6:
                        print("Esta haste não existe")
                        print("De novo")
                        break
                            
                    
            </code></pre>   
        
            <b>
                #É importante que a solução seja verificada e comprovada corretamente,
                por meio de um algoritmo.
                #Essa execução é feita percorrendo-se o algoritmo, do seu inicio ate o fim.
            </b> 
            <b>
                    Um pequeno exemplo de como é feito:
                Compraram um quantidade de canetas iguais,que foram pagas com um serto valor,
                obtendo um serto valor de troco,.Quanto custou cada caneta?
            </b>
        </div>        
        <div>
            <pre><code class="formula" contentEditable="true">    
                Formula:

                quant_X + troco = valor
                quant_X = valor - troco
                quant_X = valor_R
                X = valor_r / quant
                X = valor_unit
            </code></pre>    

            <pre><code class="modelo" contentEditable="true"> 
                Modelo:

                30x + 67 = 100
                30x = 100 - 67
                30x = 33
                x = 33/30
                x = 1.1
            </code></pre>    


            <pre><code class="python" contentEditable="true">
                Codigo em python:
            
                produto =str(input("Digite um produto : "))
                print(produto)
                quant = int(input("Digite a quantidade: "))
                print(f"{quant} unidades")
                valor = int(input("Digite um valor: "))
                print(f"{valor}$ ")
                troco = int(input("Digite o troco : "))
                print(f"{troco}$")
                qx = valor - troco
                print(f"Valor total de [{quant}] [{produto}]s é {qx}$")
                x = qx/quant
                print(f"O valor da unidade é : {x}$ ")
                
            </code></pre>
            <pre><code class="modelo" contentEditable="true"> 
                <h3>Algoritmo</h3>

               <b>INICIO</b>
                #1 Ler os valores de N,Y e Z.
                #2 Subtrair Y de z e dividir o resultado por N.
                #3 Mostrar o resultado final.
               <b>FIM</b> 
            </code></pre>    


        </div>
        
    </body>
</html>
