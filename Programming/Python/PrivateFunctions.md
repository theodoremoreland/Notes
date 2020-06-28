
# A function with  ATLEAST one underscore preceding its name can not be imported unless explicitly calling the 
# function's name (i.e. "from <module> import * " will not provide access, but "from <module> import <func>" will.)
#  Private functions created this way can also still be accessed via the syntax "<module>.<func>" if importing
# via "import <module>" syntax.

def hello():
    print("hello")

#private function
def _hello():
    print("_hello")

def __hello():
    print("__hello")

def hello__():
    print("hello__")

def __hello__():
    print("__hello__")

#private class