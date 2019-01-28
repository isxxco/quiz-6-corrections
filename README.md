2. Consider the following incomplete method.

/**
 * Precondition: values != null && values.length > 0
 */

public int mystery(int[] values) {
    int x = values[0];

    for (int value : values) {
        if (value < x) {
            x = value;    
        }
    }

    return x;
}
What does this mysterious method do?

Correct Answer:  Finds and returns the minimum value in the array. 
Why this answer is correct: The method goes through an enhanced for loop, and checks whether each value is less than a value x, which was initially assigned to the first element in the array. If the value is less, than it becomes the variable value. By the end of the loop, it returns the minimum value.


Question 5
0 / 1 pts
I need to populate an array of integers that will represent each of the perfect squares between 1 and 10. Which of the following code segments below accomplishes that task? Select all that apply.
Correct Answers:

int[] perfectSquares = new int[10];

for (int i = 1; i <= 10; i++) {
    perfectSquares[i - 1] = i * i;
}

int[] perfectSquares = new int[10];

for (int i = 0; i <= 10; i++) {
    perfectSquares[i] = (i + 1) * (i + 1);
}

int[] perfectSquares = new int[10];

int i = 1;
while (i <= 10) {
    perfectSquares[i - 1] = i * i;
}

Why these answers are correct: In the first answer choice, the array is declared and initialized. Then, using a for loop, that started with i being one and then incremented until it reaches 10, it makes the corresponding value minus one in the array squared. This is correct because since arrays are zero-indexed, and i starts with one, you have to subtract one. The second one is correct as well because it goes through the array, starting from i = 0 until i = 10. The difference here is that they add in the for loop. This is because the zero index corresponds to 1, so it has to be added this time.  The thrid answer is essentially the exact same as the first answer, just written out in a while loop instead of a for loop. 


15 Which of the following most accurately describes the code segment above and the array it modifies?
int index = 7;
values[index] = values[currentSize - 1];
values[currentSize - 1] = null;
currentSize--;

Correct Answer: The eighth object in an array is overwritten (i.e., removed) by the last object in an array. The last object in the array is set to the default value of null.

Why this answer is correct: In the second line of the code, the eighth index is given the value of the last element in the array. Then, the last elemtn in the array is then assigned the value of null, making the value null. 
