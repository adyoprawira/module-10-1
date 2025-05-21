# Module 10-1

Screenshot of Execution

![Screenshot of Execution](https://github.com/user-attachments/assets/e56f5b31-39ec-49a0-a94f-5142c874f0bc)

The "hey hey" message is printed first because it runs synchronously in main() before the executor starts processing any spawned async tasks. The async task (which prints "howdy!" and "done!") only runs after the executor is started with executor.run().
