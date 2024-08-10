
def numberToWords(number):
     num_dict = {
         0: "zero", 1: "one", 2: "two", 3: "three", 4: "four", 5: "five", 6: "six", 7: "seven", 8: "eight", 9: "nine",
         10: "ten", 11: "eleven", 12: "twelve", 13: "thirteen", 14: "fourteen", 15: "fifteen", 16: "sixteen",
         17: "seventeen", 18: "eighteen", 19: "nineteen", 20: "twenty", 30: "thirty", 40: "forty", 50: "fifty",
         60: "sixty", 70: "seventy", 80: "eighty", 90: "ninety",
         100: "one hundred", 200: "two hundred", 300: "three hundred", 400: "four hundred", 500: "five hundred",
         600: "six hundred", 700: "seven hundred", 800: "eight hundred", 900: "nine hundred",
         1000: "thousand", 1000000: "million", 1000000000: "billion"
     }

     if number in num_dict:
        return num_dict[number]
     elif number < 100:
         return num_dict[number // 10 * 10] + ' ' + num_dict[number % 10]
     elif number < 1000:
         return num_dict[number // 100] + ' hundred '+ numberToWords(number % 100)
     elif number < 1000000:
         return numberToWords(number // 1000) + ' thousand ' + numberToWords(number % 1000)
     elif number < 1000000000:
         return numberToWords(number // 1000000) + ' million ' + numberToWords(number % 1000000)
     else:
         return numberToWords(number // 1000000000) + ' billion ' + numberToWords(number % 1000000000)

 number = int(input("Enter the number: "))
 print(numberToWords(number))
