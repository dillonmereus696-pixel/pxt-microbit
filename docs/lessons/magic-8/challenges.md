input.onGesture(Gesture.Shake, function () {
    basic.clearScreen()
    randomNumber = randint(0, 4)
    if (randomNumber == 4) {
        basic.showString("DEFINITELY")
    }
    if (randomNumber == 3) {
        basic.showString("TRY AGAIN")
    }
    if (randomNumber == 2) {
        basic.showString("YES")
    } else if (randomNumber == 1) {
        basic.showString("NO")
    } else {
        basic.showString("I DON'T KNOW")
    }
    basic.showNumber(8)
})
let randomNumber = 0
basic.showString("ASK A QUESTION")
basic.showNumber(8)
input.onGesture(Gesture.Shake, () =>  {
    basic.clearScreen()
    let randomNumber = randint(0, 2)
    if (randomNumber == 2) {
        basic.showString("YES")
    } else if (randomNumber == 1) {
        basic.showString("NO")
    } else {
        basic.showString("I DON'T KNOW")

    }
    basic.showNumber(8)

})
