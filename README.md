# armstrong_query
A function created to determine whether a given number is an Armstrong number.
Belirli bir sayının Armstrong sayısı olup olmadığını belirlemek için oluşturulan bir fonksiyon.





def armstrong_query():
    el_numerico = {"1", "2", "3", "4", "5", "6", "7", "8", "9", "0"}
    number = input("Please enter a number :")
    number_set = set(number)
    total = 0
    len_num = len(number_set)
    
    if bool(number_set.difference(el_numerico)) == False:
      list(number_set)
      for j in number_set:
       total = total + int(j)**int(len_num)
    else:
      print(" It is an invalid entry. Don't use non-numeric, float, or negative values!")
      return
    if total == int(number):
      print("{} is an Armstrong number".format(number))
    else:
      print("{} is not an Armstrong number".format(number))

armstrong_query()
