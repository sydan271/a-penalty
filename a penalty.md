# a-penalty

After picking up the trash, Thanh was also punished by the teacher and had to take it out.

Building C3 has one trash room, but it is very far from the exam room. To get there, one must pass through another room. Let's temporarily call the exam room "room 1", the intermediate room "room 2", and the room containing the trash "room 3". Thanh currently has N bags of trash piled up in room 1, and wants to move these N bags to room 3. However, Thanh wants to save as much energy as possible. Each trash bag has an index representing the energy Thanh needs to use to move it from one room to another. Thanh came up with a greedy strategy as follows:

Thanh only moves the k-th trash bag from room A -> room B if and only if the k-th bag requires the most energy compared to all other bags currently in room A and room B.

For example: suppose Thanh is in room 1, with 2 trash bags having energy indices of 2 and 3. If Thanh wants to move the bag with energy 2 to room 2, he must first move the bag with energy 3 from room 2 -> room 3, and only then can he move the bag with energy 2 to room 2.

Determine, with this strategy, what is the minimum number of moves Thanh needs to make to transfer all the trash from room 1 to room 3. (Note that the path between room A and B is two-way, meaning Thanh can move the k-th bag from A -> B and vice-versa).

## Input

The first line contains T ($T \le 39$), the number of test cases. Each test case has the following format:
* The first line contains N ($N \le 1000$), the number of trash bags.
* The next line contains N numbers X ($X \le 10^6$), which are the energy indices of each trash bag. ($A[i] \ne A[j]$ for all $i \ne j$, where $A[k]$ is the energy index of the k-th bag).

## Output

For each test case, print the minimum number of moves between any two rooms if following Thanh's strategy, taking the result modulo 1000000007.

## Sample

### Input
2
1
500
2
696 969

### Output
2 8 
