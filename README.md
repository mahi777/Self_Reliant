uv=100
mv=50
name=input("Hi, what is your name? \n")
print("Hello " +name+ "! Let's play a game! \n")
print("Think of random number from 1 to 100, and I'll try to guess it!")
for i in range(1,100):
	print("\n")
	reply1=input("Is it "+str(mv)+" ? (yes/no):")
	if (reply1=="yes"):
		print("\nYeey! I got it in " + str(i) + " tries!")
		c=input("Do you want to play more(yes/no):")
		if(c=="yes"):
			continue
		else:
			print("Bye-bye")
			break
	else:
		reply2=input("\n Is the number is larger than "+str(mv)+" ? (yes/no):")
		if(reply2=="yes"):
			a=(mv+uv)//2
			mv=a+1
		else:
			b=mv//2
			mv=b

