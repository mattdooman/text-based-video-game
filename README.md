# text-based-video-game
im making a text based video game. this is my first python project ive been using pygame

weapon1 = "bow and arrows"
print("Welcome to my first game!")
name = input("What is your name? ")
age = int(input("What is your age? "))

print("Hello",name, "You are", age, "years old")

your_health = 10
speed = 5
luck = 5
defense = 3
attack = -3
hit = -2


if age >= 10:
  print("you are old enough to play! ")

  wants_to_play = input("do you want to play? ").lower()

  if wants_to_play == "yes":
    print("'You have to do your chores now, You wake up. your father's footfalls. you look out the window and get out of bed")
    print("its a beautiful day, if not a little overcast. you put on your pants, leave your room and head down the stairs ")
    print("you see your Dad and Mother at the table. Your Dad gives you a nod of good morning and your mother smiles at you. ")
    print("her smile is oddly sad, like a smile after a long hidden arguement. you grab a piece of toast and head out the door")
    take_or_leave = input("Do you take the " + weapon1 +  " take/leave?")
    if take_or_leave == "leave":
      ans = input("you leave the bow propped against the wall. you finish the toast and leave through the front door. ")
      print("you look around the familiar scene, the road that goes down to the farm is connected to your neighbors house.")
      print("while you're stretching you see soldiers coming down the road. ")
      print("You hear your parents arguing, you listen for a second. 'Well, we have to do something, it's unjust. I agree.'")
      print(" you finish.stretching and take off for the farm. as you're halfway to the farm you see the soldiers arrive")
      print(" at the enterence of the way. you wonder what that is about but you carry on. on the way to your farm, you ")
      print(" see your friend ben cutting down a tree skillfully with an ax.")
      talk_or_walk = input("do you talk to ben or keep walking? talk/walk")
      if talk_or_walk == "talk":
        ans = input("ho ben! how goes it.Ben puts down the ax. he wipes his brow and smiles at me. 'ho! how goes it? ")

    else: take_or_leave = "take"
    ans = input("you take the bow and quiver with 10 arrows. you leave the house. . While you're stretching")
    print("you see three soldiers coming down the village road. You dont pay it any mind. you begin to hear your parents arguing.")
    print("you've noticed a lot of that lately. you stay and listen a little. 'well we have to do something. i agree'   ")
    print("you stop listening, its not your business. you finish stretching and start down to the farm. The soldiers arrive at")
    print("your house and cross your path.")
    talk_or_farm = input("Do you talk to the soldiers or go on your way? talk/farm")
    if talk_or_farm == "talk":
      ans = input("you say good morning imperial soldiers. you snap the salute you were forced to learn. The soldiers")
      print("take a look at you, then look at each other. Suddenly one of them plunges their lance into your heart. you are")
      print("dead. GAME OVER")
    else: talk_or_farm = "farm"
    ans = input("You ignore them and head on your way. The soldiers look at your back walking away. 'hey you' ")
    print("you turn. 'do you live here.' you nod. the first soldier nods at the one to his left. the soldier starts after you")
    print("with murderous intent as the other soldiers continue on to your house. do you fight or flee? ")
    fight_or_flee = input("Do you fight or flee? fight/flee")
    if fight_or_flee == "fight":
      ans = input(" you nock an arrow to your bow with no hesitation. ")
      print("the soldier is a bit away from you. you aim and fire at the soldier")
      soldier_health = 2

    while True:
      import random
      options = ['hit','miss']
      hit_or_miss = random.choice(options)
      if hit_or_miss == "hit":
        print(f" he takes {hit} damage. the soldiers health is now {soldier_health + hit}")
      else: hit_or_miss = "miss"
      while  soldier_health <= 0:
        break

  while True:
    import random
    options = ['hit', 'miss']
    hit_or_miss2 = random.choice(options)
    if hit_or_miss2 == "hit":
      print(f"You took {hit} damage! Your health is now {your_health + hit}")
    else: hit_or_miss2 == "miss"
    print("the soldier missed")
    while your_health <= 0
      break

