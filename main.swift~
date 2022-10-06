import Foundation
var unsortedString = [""] 
var unsortedIntegers: [Int] = []
while let input = readLine() {
    unsortedString.append(input)
}
var i = 0
var k = 0
var x:Float = 0
for _ in unsortedString {
    for s in unsortedString[i].utf8 {
        x += Float(s)/pow((1000.0), Float(k))
        k += 1 
    }
    unsortedIntegers.append(Int(x))
    k = 0
    i += 1
    x = 0 
}
var unsortedInteger = unsortedIntegers
var z = 0
var swapcount = 0
var totalcount = 0
for num in 0..<unsortedInteger.count {
    var y = num
    while y > 0 && unsortedInteger[y] < unsortedInteger[y-1] {
        z = unsortedInteger[y] 
        unsortedInteger[y] = unsortedInteger[y-1]
        unsortedInteger[y-1] = z
        let largerString = unsortedString[y-1]
        unsortedString[y-1] = unsortedString[y]
        unsortedString[y] = largerString
     
        swapcount += 1
        totalcount += 1
        y -= 1 
    }
    swapcount = 0
}
