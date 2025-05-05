# Cifra_de_Cesar

  def Criptografia_cifra_cesar():
  	
  	alfabeto = ['a','b','c','d','e','f','g','h','i','j','k','l','m','n','o','p','q','r','s','t','u','v','w','x','y','z']
  
  	while True:
  		
  		print("="*50)
  		palavra = str(input("Digite uma palavra que deseja criptografar: ")).lower()		
  		print("="*50)	
  							
  		if palavra.isnumeric():
  			print("Digite apenas letras!")	
  			
  		else:
  			pulos = str(input("De quantas em quantas letras? "))	
  			pulos1 = int(pulos)
  			
  		print("="*50)
  		print("Palavra criptografada: ", end=" ")
  		
  		for letra in palavra:
  			if letra.isnumeric():
  				print("Não contém apenas letras! Apenas as letras serão criptografadas")
  				
  			elif letra in alfabeto:			
  				aux0 = alfabeto.index(letra)
  				aux1 = aux0 + pulos1
  				aux2 = alfabeto[aux1]			
  				print(f"{aux2}", end="")
  		print()
  		print("="*50)
  								
  Criptografia_cifra_cesar()  

