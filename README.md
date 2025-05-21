# Module 10-1

Screenshot of Execution

![Screenshot of Execution](https://github.com/user-attachments/assets/e56f5b31-39ec-49a0-a94f-5142c874f0bc)

The "hey hey" message is printed first because it runs synchronously in main() before the executor starts processing any spawned async tasks. The async task (which prints "howdy!" and "done!") only runs after the executor is started with executor.run().

#### Multiple Spawner without `drop(spawner)`

![Multiple Spawner without drop(spawner)](https://github.com/user-attachments/assets/93af96d5-c31a-4cbb-b453-1ac24b41c55a)

Without the `drop(spawner)`, the program will not end. The use of it is to tell the executor that all tasks have been run and to stop the spawners. As seen on the screenshot, the program just waits.
