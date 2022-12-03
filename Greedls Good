function score(dice) {
    console.log(dice);
    let total = 0;
    let unique = [...new Set(dice)];
    for (i = 0; i < unique.length; i++) {
        function checkDice(number) {
            return number == unique[i];
        }
        console.log(dice.filter(checkDice));
        const diceFilterLength = dice.filter(checkDice).length;
        console.log("Number: " + unique[i]);
        console.log("Length: " + dice.filter(checkDice).length);
        console.log("Divisible by: " + diceFilterLength / 3);
        console.log("Remainder of: " + diceFilterLength % 3);
        if (unique[i] === 1 && Math.floor(diceFilterLength / 3)) {
            total += Math.floor(diceFilterLength / 3) * 1000;
        } else if (unique[i] === 6 && Math.floor(diceFilterLength / 3)) {
            total += Math.floor(diceFilterLength / 3) * 600;
        } else if (unique[i] === 5 && Math.floor(diceFilterLength / 3)) {
            total += Math.floor(diceFilterLength / 3) * 500;
        } else if (unique[i] === 4 && Math.floor(diceFilterLength / 3)) {
            total += Math.floor(diceFilterLength / 3) * 400;
        } else if (unique[i] === 3 && Math.floor(diceFilterLength / 3)) {
            total += Math.floor(diceFilterLength / 3) * 300;
        } else if (unique[i] === 2 && Math.floor(diceFilterLength / 3)) {
            total += Math.floor(diceFilterLength / 3) * 200;
        };

        if (unique[i] === 1 && diceFilterLength % 3) {
            total += (diceFilterLength % 3) * 100;
        } else if (unique[i] === 5 && diceFilterLength % 3) {
            total += (diceFilterLength % 3) * 50;
        }
        console.log("Total: " + total);
    }
    console.log("Subtotal: " + total);
    return total;
}