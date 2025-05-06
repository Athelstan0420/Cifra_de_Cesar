# Cifra_de_Cesar

    def Criptografia_cifra_cesar():
    
    	print(	
    		
    		"""
    		Bem vindo! Criptografe palavras ou frases aqui utilizando criptografia cimétrica. 
    
    		AVISO: Digite apenas letras! números não serão aceitos. 
    
    		"""
    	   
    	    )
    
    	alfabeto = ['a','b','c','d','e','f','g','h','i','j','k','l','m','n','o','p','q','r','s','t','u','v','w','x','y','z']
    	numeros = ['0','1','2','3','4','5','6','7','8','9']	
    
    	palavra = str(input("Digite uma palavra que deseja criptografar: ")).lower()		
    	oq_quis = palavra	
    	
    	pulos = ''
    	while pulos not in numeros:					
    		pulos = str(input("De quantas em quantas letras? "))
    		for i in pulos:
    			if i not in alfabeto:
    				print("Digite apenas números! ")
    	pulos1 = int(pulos)
    
    	oq_obteve = []
    	print("Palavra criptografada: ", end=" ")	
    	for letra in palavra:
    		if letra in alfabeto:			
    			aux0 = alfabeto.index(letra)
    			aux1 = aux0 + pulos1
    			aux2 = alfabeto[aux1]
    			oq_obteve.append(aux2)
    			print(f"{aux2}", end="")
    			
    	print()
    	print(f"O que você digitou: ({oq_quis})", end='')	
    	print(" - o que retornou: ",end='')	
    	print("(", end='')		
    	for l in oq_obteve:
    		print(l, end='')	
    	print(")")			
    	# print()
    
    Criptografia_cifra_cesar() 

