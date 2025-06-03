## 🧠 Function Explanation: result(sentences)

The result function here is used to find the maximum number of words from a list of sentences.

### 📌 Example:

Given the following sentences:

```javascript
const sentences = [
'Mauris ultricies sed sapien eget malesuada. Suspendisse et aliquet odio, id ultrices erat. Praesent vehicula erat nulla. Aliquam a lorem urna. Donec.',
'Duis at tellus et ex bibendum pellentesque sed in nibh. Sed aliquet, diam id mollis facilisis, massa metus accumsan elit, at mattis magna.',
'Sed non nibh quam. Pellentesque eget ultrices diam. Aliquam diam justo, consectetur ac dui lobortis, vestibulum bibendum lorem. Sed porta pulvinar.',
];
```


The function will return 23 because "Mauris ultricies sed sapien eget malesuada. Suspendisse et aliquet odio, id ultrices erat. Praesent vehicula erat nulla. Aliquam a lorem urna. Donec." has the most words (23).

### 👉 How it works:

It starts by setting variable maxWords to 0:
```javascript
function result(sentences) {
  let maxWords = 0;
	
}
```
Then, it loops through each sentence in the array using .forEach():
```javascript
function result(sentences) {
  let maxWords = 0;
	
  sentences.forEach(sentence => {
    
  })
}
```
For each sentence, it splits the sentence into words using .split(' ').
It counts how many words are in the sentence:

```javascript
function result(sentences) {
  let maxWords = 0;
	
  sentences.forEach(sentence => {
    const maxCount = sentence.split(' ').length;
		
  })
}
```
If the current sentence has more words than maxWords, it updates maxWords:
```javascript
function result(sentences) {
  let maxWords = 0;
	
  sentences.forEach(sentence => {
    const maxCount = sentence.split(' ').length;
    if( maxCount > maxWords){
        maxWords = maxCount;
    }
  })
  
}
```
After checking all the sentences, it returns the highest word count found.
```javascript
function result(sentences) {
  let maxWords = 0;
	
  sentences.forEach(sentence => {
    const maxCount = sentence.split(' ').length;
    if( maxCount > maxWords){
        maxWords = maxCount;
    }
  })
  return  maxWords;
}
```

### 🚀 How to Use

Clone this repository
First, download the project to your local machine by using this command:

```bash
git clone <your-repo-url>
```

Replace <your-repo-url> with the actual link to your GitHub repo.

Go to the project folder
```bash
cd <your-project-folder>
```

Start the app
Run the program with:
```bash
npm run start

or

node index.js
```


See the result The result will be printed in your terminal/console.

### ✅ Use case:
This is helpful if you want to know which sentence is the longest in terms of word count.