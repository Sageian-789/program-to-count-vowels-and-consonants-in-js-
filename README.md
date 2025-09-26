# program-to-count-vowels-and-consonants-in-js-
function countVowelsAndConsonants(str) {
    
    str = str.toLowerCase();

    let vowels = 0;
    let consonants = 0;

    const vowelSet = "aeiou";

    for (let i = 0; i < str.length; i++) {
        let ch = str[i];
        
        if (ch >= 'a' && ch <= 'z') {
            if (vowelSet.includes(ch)) {
                vowels++;
            } else {
                consonants++;
            }
        }
    }

    console.log(`Vowels: ${vowels}`);
    console.log(`Consonants: ${consonants}`);
}


countVowelsAndConsonants("Hello World");
