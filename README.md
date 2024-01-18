# lmao
i lost all my old code so im not making the same mistake twice 
const readlineSync = require('readline-sync');

function displayLinkInfo() {
    console.log("Welcome to the Legend of Zelda Information Center!");
    console.log("===============================================");

    // Get user input for Link's game
    const gameChoice = readlineSync.keyInSelect(['Breath of the Wild', 'Tears of the Kingdom'], 'Choose a game for Link:');
    
    if (gameChoice === -1) {
        console.log("Goodbye!");
        return;
    }

    let linkInfo = {};

    // Set Link's information based on the selected game
    switch (gameChoice) {
        case 0: // Breath of the Wild
            linkInfo.name = "Link";
            linkInfo.game = "The Legend of Zelda: Breath of the Wild";
            linkInfo.abilities = ["Master Sword", "Hylian Shield", "Runes", "Paraglider"];
            linkInfo.feats = ["Defeating Calamity Ganon", "Restoring Hyrule"];
            break;

        case 1: // Tears of the Kingdom
            linkInfo.name = "Link";
            linkInfo.game = "The Legend of Zelda: Tears of the Kingdom";
            linkInfo.abilities = ["ultra hand and auto build 1", "acend 2", "reverse 3"];
            linkInfo.feats = ["defating all of ganndofs monsters and forming the new team of sages ", "defating demon king ganndorf restoring hyrule and saving princess zelda "];
            break;

        default:
            break;
    }

    // Display Link's information
    console.log("\nLink's Information");
    console.log("==================");
    console.log(`Name: ${linkInfo.name}`);
    console.log(`Game: ${linkInfo.game}`);
    console.log(`Abilities: ${linkInfo.abilities.join(', ')}`);
    console.log(`Feats: ${linkInfo.feats.join(', ')}`);
}

// Run the program
displayLinkInfo();
code 1



const readlineSync = require('readline-sync');

function displayLinkInfo() {
    console.log("Welcome to the Legend of Zelda Information Center!");
    console.log("===============================================");

    const gameChoice = readlineSync.keyInSelect(['Breath of the Wild', 'Tears of the Kingdom'], 'Choose a game for Link:');
    
    if (gameChoice === -1) {
        console.log("Goodbye!");
        return;
    }

    let linkInfo = {};

    switch (gameChoice) {
        case 0: // Breath of the Wild
            linkInfo.name = "Link";
            linkInfo.game = "The Legend of Zelda: Breath of the Wild";
            linkInfo.abilities = ["Master Sword", "Hylian Shield", "Runes", "Paraglider"];
            linkInfo.feats = ["Defeating Calamity Ganon", "Restoring Hyrule"];
            linkInfo.masterSwordInfo = {
                origin: "Created by the goddess Hylia",
                significance: "Blade of Evil's Bane, repels evil forces",
                awakening: "Unlocked by proving one's courage",
                upgrades: "Can be enhanced through quests",
                energySource: "Connected to the Great Deku Tree in Breath of the Wild",
                limitations: "Needs time to recharge in Breath of the Wild",
            };
            break;

        case 1: // Tears of the Kingdom
            linkInfo.name = "Link";
            linkInfo.game = "The Legend of Zelda: Tears of the Kingdom";
            linkInfo.abilities = ["New Ability 1", "New Ability 2", "New Ability 3"];
            linkInfo.feats = ["New Feat 1", "New Feat 2"];
            linkInfo.masterSwordInfo = {
                origin: "Customize based on the game's lore",
                significance: "Define based on the game's story",
                awakening: "Define based on the game's plot",
                upgrades: "Define based on the game's mechanics",
                energySource: "Define based on the game's lore",
                limitations: "Define based on the game's mechanics",
            };
            break;

        default:
            break;
    }

    console.log("\nLink's Information");
    console.log("==================");
    console.log(`Name: ${linkInfo.name}`);
    console.log(`Game: ${linkInfo.game}`);
    console.log(`Abilities: ${linkInfo.abilities.join(', ')}`);
    console.log(`Feats: ${linkInfo.feats.join(', ')}`);

    console.log("\nMaster Sword Information");
    console.log("========================");
    console.log(`Origin: ${linkInfo.masterSwordInfo.origin}`);
    console.log(`Significance: ${linkInfo.masterSwordInfo.significance}`);
    console.log(`Awakening: ${linkInfo.masterSwordInfo.awakening}`);
    console.log(`Upgrades: ${linkInfo.masterSwordInfo.upgrades}`);
    console.log(`Energy Source: ${linkInfo.masterSwordInfo.energySource}`);
    console.log(`Limitations: ${linkInfo.masterSwordInfo.limitations}`);
}

displayLinkInfo();
code 2







const readlineSync = require('readline-sync');

function add(x, y) {
    return x + y;
}

function subtract(x, y) {
    return x - y;
}

function multiply(x, y) {
    return x * y;
}

function divide(x, y) {
    if (y !== 0) {
        return x / y;
    } else {
        return "Error: Division by zero";
    }
}

function calculator() {
    console.log("Welcome to the Simple Calculator!");
    console.log("=================================");

    const num1 = parseFloat(readlineSync.question("Enter the first number: "));
    const operator = readlineSync.question("Enter the operator (+, -, *, /): ");
    const num2 = parseFloat(readlineSync.question("Enter the second number: "));

    let result;

    switch (operator) {
        case '+':
            result = add(num1, num2);
            break;
        case '-':
            result = subtract(num1, num2);
            break;
        case '*':
            result = multiply(num1, num2);
            break;
        case '/':
            result = divide(num1, num2);
            break;
        default:
            console.log("Invalid operator. Please use +, -, *, or /.");
            return;
    }

    console.log(`Result: ${result}`);
}

// Run the calculator
calculator();
code 3





const readlineSync = require('readline-sync');

function getEmbarrassingSituation() {
    return readlineSync.question('Can you share a recent embarrassing situation? ');
}

function giveAdvice() {
    console.log('\nHere\'s some friendly advice:');
    console.log('1. Remember, everyone makes mistakes, and embarrassing moments happen to everyone.');
    console.log('2. Laugh it off! Sometimes, humor is the best way to deal with embarrassing situations.');
    console.log('3. Learn from it. Use the experience to grow and become more resilient.');
    console.log('4. Don\'t be too hard on yourself. Were all human!');
}

function main() {
    console.log('Welcome to the Embarrassing Situation Advisor!');
    
    const embarrassingSituation = getEmbarrassingSituation();
    
    console.log('\nOh, that sounds embarrassing! Let me offer you some advice.');

    giveAdvice();

    console.log('\nI hope that helps! Feel free to come back if you need more advice. Have a great day!');
}

main();




function getEmbarrassingSituation() {
    return readlineSync.question('Can you share a recent embarrassing situation? ');
}

function giveGeneralAdvice() {
    console.log('\nHere\'s some general advice:');
    console.log('1. Remember, everyone makes mistakes, and embarrassing moments happen to everyone.');
    console.log('2. Laugh it off! Sometimes, humor is the best way to deal with embarrassing situations.');
    console.log('3. Learn from it. Use the experience to grow and become more resilient.');
    console.log('4. Don\'t be too hard on yourself. We\'re all human!');
}

function giveSpecificAdvice(situation) {
    console.log(`\nHere's some advice specifically for dealing with "${situation}":`);
    // Add specific advice for dealing with the provided embarrassing situation
    console.log('...');
}

function main() {
    console.log('Welcome to the Embarrassing Situation Advisor!');
    
    const embarrassingSituation = getEmbarrassingSituation();
    
    console.log('\nOh, that sounds embarrassing!');

    const wantSpecificAdvice = readlineSync.keyInYNStrict('Would you like specific advice on how to deal with this situation?');

    if (wantSpecificAdvice) {
        giveSpecificAdvice(embarrassingSituation);
    } else {
        giveGeneralAdvice();
    }

    console.log('\nI hope that helps! Feel free to come back if you need more advice. Have a great day!');
}

main();
code 4
