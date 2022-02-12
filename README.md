# CommaCode
Write a function that takes a list value as an argument and returns a string with items separated by commas and "and" before the last item. 

myFavoriteAlbums = ['How to be a Human Being',
                    'Three Cheers for Sweet Revenge',
                    'Closer',
                    'From Under the Cork Tree',
                    'Pretty. Odd.']
                    

olympics = ['figure skating', 'bobsled', 'ski']

empty_list = []

def returnString(enterList):
    try: 
        for title in range(len(enterList)-1):
            print(str(enterList[title]), end = ', ')
    
        print( 'and, ' + enterList[-1])
    
    except IndexError:
        print('This list has no items!')
    

returnString(olympics)
