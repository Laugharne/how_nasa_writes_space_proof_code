# [](https://youtu.be/GWYhtksrmhE?t=0) Introduction to NASA's Code Rules

```
This is a transcription of a YouTube video, which I found particularly relevant.
```

**Section Overview**: In this section, we learn about the importance of writing reliable and safe code for production environments, particularly in scenarios involving extreme safety measures. We explore **NASA's set of rules** known as the *"Power of 10"* that are derived from their experience in developing software for space missions.

- [00:00](https://www.youtube.com/watch?v=GWYhtksrmhE&t=0s) Introduction
- [00:44](https://www.youtube.com/watch?v=GWYhtksrmhE&t=44s) #01 Simple Control Flow
- [01:08](https://www.youtube.com/watch?v=GWYhtksrmhE&t=68s) #02 Limit All Loops
- [01:40](https://www.youtube.com/watch?v=GWYhtksrmhE&t=100s) #03 Don't use the Heap
- [02:15](https://www.youtube.com/watch?v=GWYhtksrmhE&t=135s) #04 Limit Function Size
- [03:01](https://www.youtube.com/watch?v=GWYhtksrmhE&t=181s) #05 Practice Data Hiding
- [03:27](https://www.youtube.com/watch?v=GWYhtksrmhE&t=207s) #06 Check Return Values
- [04:17](https://www.youtube.com/watch?v=GWYhtksrmhE&t=257s) #07 Limit the Preprocessor
- [04:57](https://www.youtube.com/watch?v=GWYhtksrmhE&t=297s) #08 Restrict Pointers Use
- [05:33](https://www.youtube.com/watch?v=GWYhtksrmhE&t=333s) #09 Be Pedantic
- [05:47](https://www.youtube.com/watch?v=GWYhtksrmhE&t=347s) test test test
- [05:55](https://www.youtube.com/watch?v=GWYhtksrmhE&t=355s) Interaction Reminder


## NASA's Code Rules

- [00:19](https://youtu.be/GWYhtksrmhE?t=19) **The Power of 10**: NASA has a set of rules called the Power of 10, which focuses on making code easy to statically analyze.
- [00:37](https://youtu.be/GWYhtksrmhE?t=37) **Simple Control Flow Constructs**: NASA **restricts** the use of **goto** statements, **setjump**, **longjump**, and **recursion** to ensure clear and understandable control flow graphs.
- [00:58](https://youtu.be/GWYhtksrmhE?t=58) **Fixed Upper Bound for Loops**: All loops in NASA's code have a fixed upper bound to prevent runaway code and crashes.
- [01:18](https://youtu.be/GWYhtksrmhE?t=78) **Exclusive Use of Stack Memory**: NASA recommends **avoiding** the use of **heap memory** and **garbage collectors** to eliminate memory bugs. By using stack memory exclusively, they can predict exactly how much memory their program will use.
- [01:57](https://youtu.be/GWYhtksrmhE?t=117) **Functions with Single Responsibility and Limited Size**: Functions should do one thing and be **no longer than 60 lines** or about the size of a piece of paper. This ensures readability, understandability, and testability as a single unit.
- [02:50](https://youtu.be/GWYhtksrmhE?t=170) **Data Hiding at Lowest Scope Possible**: Variables should be declared at the **lowest scope required** to reduce access points and potential debugging issues.
- [03:28](https://youtu.be/GWYhtksrmhE?t=208) **Check Return Values for Non-Void Functions**:
  - All return values for **non-void functions** should be checked to ensure proper behavior.
  - **Ignored return values** should be explicitly cast to a void type.
- [04:25](https://youtu.be/GWYhtksrmhE?t=265) **Limited Use of C Preprocessor**: NASA limits the use of the C preprocessor to file inclusions and simple conditional macros to maintain code clarity and **avoid obfuscation**.
- [05:03](https://youtu.be/GWYhtksrmhE?t=303) **Restriction of Pointer Use**: Pointers should not be dereferenced more than one layer at a time to prevent misuse and promote proper structuring.
- [05:22](https://youtu.be/GWYhtksrmhE?t=322) **No Function Pointers**: Function pointers obfuscate the code control flow graph of your program and make it very hard to statically analyze and fully test.

# [05:41](https://youtu.be/GWYhtksrmhE?t=341) Ensuring Code Quality and Testing

**Section Overview**: This section emphasizes the importance of ensuring code quality and conducting thorough testing before launching a project.

## Analyzing Code with Static Code Analyzers

- It is crucial to **analyze** your code using **multiple static code analyzers** with different rule sets.
- This practice helps identify and address any potential problems or errors in the code.
- By utilizing various analyzers, you can ensure that every possible issue is detected and treated as an error.

## Unit Testing for Code Validation

- Another essential step is to perform **unit testing** on your code.
- Unit tests help validate the functionality of individual units or components of the code.
- Through unit testing, you can verify that each part of your code works correctly and produces the expected results.

## Importance of Code Quality Assurance

- Prioritizing code quality assurance is vital before launching any project.
- By thoroughly analyzing and testing your code, you can minimize the risk of encountering issues or bugs later on.
- Ensuring high-quality code increases reliability, maintainability, and overall performance.

## Conclusion

Before launching a project, it is crucial to prioritize code quality by analyzing it with static code analyzers, conducting unit tests, and implementing proper quality assurance measures. These steps help identify and address potential issues early on, ensuring a more reliable and robust final product.

[Generated with Video Highlight](https://videohighlight.com/video/summary/GWYhtksrmhE)


