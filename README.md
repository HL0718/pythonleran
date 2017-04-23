
#encoding:utf-8
print set('abcd')  # set(['a', 'c', 'b', 'd'])
print set(['nice', 'to', 'meet', 'to'])
firstSet = set([1, 2, 3])
secondSet = set([3, 4, 5])
print firstSet & secondSet
print firstSet | secondSet
print firstSet - secondSet
items = [('name', 'Mike'), ('age', '20')]
itemDict = dict(items)

list = ([20, 'age'], ['Mike', 'name'])
ddict = dict(list)

dict = {'name': 'YingYing', 'password': 233}

emptyDict = {}
fDict = {}.fromkeys(('id', 'score'))
print fDict
formDict = {}.fromkeys(('x', 'y'), (-1, -2))
print formDict
for key in dict.keys():
    print key
    for value in dict.values():
        print value

if 'name' in ddict.values():
    print 'name in ddict'
    print ddict.has_key(20)
    print itemDict['name']
    print itemDict.get('name')
    itemDict['name'] = 'Lily'
    del itemDict['name']
    itemDict.clear()
    dict = {'name': 'shaBi', 'age': 20}
    print 'I have a friend named %(name)s, he is %(age)s years old' % dict


    print abs(-2)
    print cmp(1,2),cmp(2,1),cmp(3,3)
    print int("123")


    def my_abs(a, b):
        if a > b:
            return 1
        else:
            if a < b:
                return -1
            else:
                return 0
    print my_abs(7, -4)


def power(x, n=2):
    s = 1
    while n > 0:
        n -= 1
        s *= x
    return s
print power(2),power(2,4)
class people():
    def __init__(self,name,hair,height):
        self.name=name
        self.hair=hair
        self.height=height
    def printName(self):
        print 'my name is',self.name
    def printHair(self):
        print 'I have hair'
    def printHeight(self):
        print 'I have height'
Mike=people('Mike','short','tall')
Mike.printName()
Mike.printHair()

class boy(people):

    def printName(self):
        print 'I have my own name, my name is ', self.name


Mike = boy('Mike', 'short', 'tall')
Mike.printName()




# pythonleran
