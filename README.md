# Python-Software-related-questions
Question 1 - Have you ever worked on any networking related program (whether in python or any other language). Networking means working with TCP/UDP.

Answer- no, not yet. TCP socket creation is what I am looking forward to work on.

Question 2 - Do you have any knowledge or experience with SIP (session initiation protocol). Again this experience does not necessarily need to be in python.

Answer- I have basic knowledge regarding SIP as it was in my course in computer networking. However, I haven’t implemented it in any programming language yet.

Question 3 - Do you have knowledge of databases (either NoSQL or SQL). Which ones?
Answer- yes, I have studied SQL and have complete knowledge about the commands associated to it.

Question 4 - Have you ever worked with an ORM like sqlalchemy/mongoengine in python.
Answer- no but I have worked on postgresql.

Question 5 - Have you ever worked with any microservices/web-based frameworks in python (like Flask/Sanic/Django).
Answer- yes, Django. I have created website using Django and still working on this to improve my skills.

Question 6 - Have you ever used any concurrency framework like asyncio/gevents/twisted in python? If yes, which ones.
Answer- NO. I have no idea about this.




Python Exercises
Exercise 2
Agent selector program


import random
def employee(available_since, **data):
    
    issues= ['sales', 'marketing', 'content', 'language', 'support']
    
    for name, job in data.items():
            print('{} is from {} department ' .format(name,job))
    for i in issues:
      if i == job:
        print(data[name])
        
    print('available since  ' + str(available_since) + '  hours')
    if available_since >=5 and available_since <=8 :
            print("all available")
            print( bool(input('Will you like to Opt. this Issue? Yes or No')))
    elif available_since >=2 and available_since <=4 :
        print('Least Busy')
        is_available= False 
        s= str(input('Are you available? press 1 for yes and 0 for No! '))
        def one():
          return "yes"
          for i in issues:
            if i == data.job:
              print('assigned')
        def zero():
          return "no"
        def nmu_to_str(argument):
          switcher ={
            yes: 1,
            no: 0
          }
          func = switcher.get(argument, lambda: "Invalid")
          print (func)
        
        
        
    else:
        print (random.choice(list(data)))

name= (input('enter  employee names:  '))
job= (input('enter  job field '))
available_since =  int(input('Enter time since you are free  '))
data = {}
data[name] = job
employee(available_since,**data)

