# Line Comments Aligner

This standalone HTML tool aligns line comments in text (code) files. It's a simple utility that can be run locally in your web browser.

---

## How to Use

1. **Open the HTML File**: Download the HTML file and open it in your web browser or [run it directly](https://danebae.github.io/aligner) from GitHub.

2. **Specify Parameters**: 
   - Enter the comment string you want to use (e.g., "//", "#", etc.) in the "Comment String" field.
   - Specify the alignment position for comments by entering a number in the "Alignment Position for Comments" field.

3. **Choose Files**: Click on the "Choose Files" button to select one or multiple text files you want to process.

4. **Process Files**: Click on the "Process Files" button. The tool will process the selected files, aligning the comments as per your specifications.

5. **Download Modified Files**: After processing, the modified files will be automatically downloaded to your default download folder.

---

## Expected Output

- Comments prefixed by the chosen string will be aligned to the specified position.
- Alignment will be achieved by adding or removing spaces before comments.
- Comments in lines without code will remain unchanged.
- Original files will not be modified; modified files will be downloaded to your download folder.

---

## Example

Suppose you have a text file named `example.txt` with the following content:

```javascript
// This comment has no code so it will be unchanged
    // This comment has no code either; it will be unchanged as well
function someFunction() {
    let a = 20; // This is a line comment
    return a;         // This is another line comment
}
```

If you specify "//" as the comment string and 40 as the alignment position, the output file after processing example.txt would contain:

```javascript
// This comment has no code so it will be unchanged
    // This comment has no code either; it will be unchanged as well
function someFunction() {
    let a = 20;                        // This is a line comment
    return a;                          // This is another line comment
}
```
