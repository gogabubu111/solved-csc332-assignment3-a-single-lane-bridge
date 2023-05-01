Download Link: https://assignmentchef.com/product/solved-csc332-assignment3-a-single-lane-bridge
<br>
A single-lane bridge connects the two Vermont villages of North Tunbridge and South Tunbridge. Farmers in the two villages use this bridge to deliver their produce to the neighboring town. The bridge can become deadlocked if a northbound and a southbound farmer get on the bridge at the same time. (Vermont farmers are stubborn and are unable to back up.)

Implement a solution using Pthreads that synchronizes the threads access to the output screen and prevents deadlock. In particular, represent northbound and southbound farmers as separate threads (use several threads representing the northbound and southbound farmers). Once a farmer is on the bridge the associated thread will:

<ul>

 <li>Print to the screen “North (or South) Tunbridge farmer can cross the bridge” after the thread has granted access to the lock.</li>

 <li>Print on the screen “North (or South) Tunbridge is traveling on the bridge…” as</li>

 <li>Sleep for a random period (up to 3 seconds).</li>

 <li>Print to the screen “North (or South) Tunbridge farmer has left the bridge” before releasing the lock.</li>

</ul>

Meanwhile, the other village farmer is waiting for the bridge to be clear. The program screen printout should look like the following:

North Tunbridge #1 farmer can cross the bridge

North Tunbridge #1 is traveling on the bridge…

North Tunbridge #1 farmer has left the bridge




South Tunbridge #1 farmer can cross the bridge South Tunbridge #1 is traveling on the bridge…

South Tunbridge #1 farmer has left the bridge




North Tunbridge #2 farmer can cross the bridge

North Tunbridge #2 is traveling on the bridge…

North Tunbridge #2 farmer has left the bridge

Submit the following:

<ol>

 <li>The program code with all comments</li>

 <li>Screenshots of the output for your program when:

  <ol>

   <li>not using the lock</li>

   <li>using the lock</li>

  </ol></li>

</ol>

<ul>

 <li>Assignment report which will answer the following questions:

  <ol>

   <li>What type of lock your code is using?</li>

   <li>How many processes does your program fork? Are there equal number of North and South processes?</li>

  </ol></li>

</ul>