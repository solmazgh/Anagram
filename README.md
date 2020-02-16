# Anagram
# check two string to be anagram 



function anagrams(stringA, stringB) {

    //Sanitize input string
    stringA = stringA.toLowerCase().replace(/[\W_]+/g, "");
    stringB = stringB.toLowerCase().replace(/[\W_]+/g, "");
    
    //sort two string
    const stringAsorted = stringA.split("").sort().join("");
    const stringBsorted = stringB.split("").sort().join("");

    return stringAsorted === stringBsorted;
}
