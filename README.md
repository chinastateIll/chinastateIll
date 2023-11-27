### Actually I just have began learning a python.lang


def data(): 
    name=(input("Your Nickname: \n"))
    array = False
    while not array:
            try:
                age=int(input("Your age: \n"))
                array = True 
            except ValueError:
                print('Dude, you must enter a number in age-field. Try again. ')
    return {'name': name, 'age': age}
       
user = data()

def doebis_do_vozrasta():
    if user['age'] > 18:
        print('Ого, похоже ты уже взрослый. Гы-гыг 🦖 \n')
    else:
        print('Юн и полон сил, значит? Хе-хе \n')
        
doebis_do_vozrasta()

def say_hello():
      print(f"So! \nHi there,  {user['name']} 🙂 \n\nHere we have been testing the loop-function. \nSuggest you to take a part. \nRight?")
      
say_hello()

def choice():
    resp = None
    
    while resp not in ['1', '2']:
        resp = input("1. Yes. \n2. No. \n")
    
        if resp == '1':
            print("Okey, let's do it! ")
        elif resp == '2':
            print("Well done!")
        else:
            print("This option is not provide. Please, select the number of answer again.")
            
choice() 
