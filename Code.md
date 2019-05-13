# Geometric-and-Other-Calculator
A geometric Calculator I have created for a project. I am new to python
print("Possible Inputs - Cylinder, Cube, Triangle Prism, sphere, Trapezoid, Interest, Calculator")
s = input("Calculate - ")
s = s.lower()
print(s)
if s == "cylinder":
  print("Possible Inputs - Area, Total surface, lateral surface, volume")
  t = input("Math Type - ")
  print("Cylinder -", t)
  r = float(input("radius - "))
  h = float(input("height - "))
  t = t.lower()
  if t=="area":
    print("Area = " + str(3.14*r**2*h))
  elif t=="total surface":
    print("Total Surface Area = " + str(2*3.14*r*h + 2*3.14*r**2))
  elif t=="lateral surface":
    print("Lateral Surface Area = "+str(2*3.14*r*h))
  elif t=="volume":
    print("Volume - "+str(2*3.14*r**2*h))
  else:
    print("Invalid Information")
elif s=="cube":
  print("Possible Inputs - Area, Total Surface, Lateral Surface, Volume")
  t = input("Math Type - ")
  print("Cube - "+ str(t))
  l = float(input("length- "))
  w = float(input("Width- "))
  h = float(input("Height-"))
  t = t.lower()
  if t=="area" :
      print("Area - "+str(l*w))
  elif t=="total surface":
    print("Total Surface Area - "+str(w+w+l+l*h + 2*l*w))
  elif t=="lateral surface":
      print("Lateral Surface Area - "+str(w+w+l+l*h))
elif s=="triangle":
  print("Possible Inputs - Area, total Surface, Lateral Surface, Volume")
  t = input("Math Type - ")
  print("Triangle - "+str(t))
  s1 = float(input("Side One -  "))
  s2 = float(input("triangle base - "))
  b = float(input("Side Three - "))
  h = float(input("Triangle Height -"))
  a = float(input("Prism Height - "))
  t = t.lower()
  if t=="area":
      print("Area - "+str(b*h/2))
  elif t=="total surface":
    print("Total Surface Area - "+str(s1+s2+b*a+2*b*h/2))
  elif t=="lateral surface":
      print("Lateral Surface Area"+str(s1+s2+b*a))
  elif t=="volume":
    print("Volume - "+str(b*h*a))
  else:
      print("Invalid Infomation")
elif s=="calculator":
  print("Possible Inputs - x for multiplication, / for division, + for Addition, - for subtraction")
  t = input("Math Type - ")
  if t == "x" or t == "*":
    f = "Multiplication"
  elif t == "/":
    f = "division"
  elif t == "+":
    f = "Addition"
  elif t == "-":
    f = "Subtraction"
  else:
    print("Invalid Information")
  b = float(input("First digit - "))
  v = float(input("second digit -"))
  print("Calculator - "+str(f))
  if t=="x":
    print(b*v)
  elif t== "/":
    print(b/v)
  elif t== "+":
    print(b+v)
  elif t== "-":
    print(b-v)
elif s== "sphere":
  print("Possible Inputs - Volume, Surface, Area")
  t = input("Caculate - ")
  t = t.lower()
  if t== "volume":
    print("Volume\n")
    f = "v"
  elif t== "surface":
    print("Surface Area")
    f = "t"
  elif t== "area":
    print("Circle Area")
    f = "a"
  r = float(input("Radius - "))
  print(r)
  if f == "v":
    print("Volume - " + str(4/3*3.14*r**3))
  elif	 f == "t":
    print("Sphere Surface Area - " + str(4*3.14*r**2))
  elif f== "a":
    print(" Circle Area - " + str(3.14*r**2))
elif s== "trapezoid":
  print("Possible Inputs - Area, Volume")
  t = input("Math Type - ")
  t = t.lower()
  a = float(input("Top Base - "))
  b = float(input("Lower Base - "))
  h = float(input("height - "))
  if t=="area":
    area = ((a + b) / 2) * h
    print("Area - ", area)
  elif t=="volume":
    l = float(input("length - "))
    area = ((a + b) / 2) * h
    print("Volume - ", area*l)
elif s=="interest":
  print("Possibly inputs - Simple, Compound")
  t = input("Math Type - ")
  t = t.lower()
  if t== "simple":
    print("possibly inputs - Interest")
    print("Simple Interest - " + str(p*r*t))
    print("Total Amount - " + str((p*r*t)+ p))
else:
  print("Invalid Input, Please input information correctly")
