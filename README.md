# csc258-lab-5-clocks-and-counters-solved
**TO GET THIS SOLUTION VISIT:** [CSC258 Lab 5-Clocks and Counters Solved](https://www.ankitcodinghub.com/product/csc258-lab-5-solved-2/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;117506&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;3&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (3 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSC258 Lab 5-Clocks and Counters Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (3 votes)    </div>
    </div>
1 Learning Objectives

The purpose of this lab is to learn how to create counters and to be able to control when operations occur at high clock speeds.

2 Marking Scheme

This lab, like other labs, is worth 6% of your final grade, broken down as follows:

• Part II (in-lab): 1 mark

3 What You Need To Do

3.1 Preparation Before the Lab

You are required to complete Parts I to III of the lab by building and testing circuits in Logisim. Include your schematics and Logisim files for Parts I to III in your prelab. You must simulate your circuit inside Logisim, but since the Logisim test vectors only handle combinational circuits, your prelab report will include a test plan and important test cases (which will be tested in your demo). You should also answer the questions in the handout that are marked as (PRELAB).

3.2 In-lab Work

You are required to implement and test all of Parts I to III of the lab. You need to demonstrate all parts to the teaching assistants.

3.3 Summary of Lab Requirements

The following is a summary of what you need to perform for this lab (and labs in general):

• Make sure to include the following in the pre-lab report:

– Answers to any question posed in the prelab sections

– Diagrams of your circuit designs (when asked)

– Any .circ files that you created to implement your designs

– Test vector files (when possible). Note: test vectors don’t work on sequential circuits, but some components (such as your LUT) are combinational circuits that can be tested more effectively with test vectors.

– Screenshots of your circuit’s performance (when test vectors aren’t possible). Since you’re only meant to include a sample of the possible test cases here, consider which input combinations would best illustrate the behaviour of your circuit.

• What to do in demo sessions:

– Review your pre-lab report (as necessary)

– Running and simulating your designs, using the Poke tool and/or test vectors

– Answer questions about your design and/or the handout

• Files required to upload:

– Pre-lab report (including circuit diagrams, answers to questions, etc)

– Logisim files (.circ)

– Test vectors (.txt)

4 Part I

Consider the circuit in Figure 1. It is a 4-bit synchronous counter that uses four T-type flip-flops. The counter increments its value on each positive edge of the clock if the Enable signal is 1 (i.e. high). The counter is reset to 0 by setting the Clear b signal low, which means that the clear is an active-low asynchronous clear. (In Logisim, all the input signals are asynchronous active high by default.) You should implement an 8-bit version of this counter.

Figure 1: A 4-bit counter.

An asynchronous clear means that as soon as the Clear b signal changes (here from 1 to 0 since we have an active-low signal), irrespective of whether this change happened at the positive clock edge or not, the T flip-flop should be reset. This is in contrast to the synchronous reset, where the D flip-flop can only be reset at the positive edge of the clock.

For this part, perform the following steps:

1. Draw the schematic for an 8-bit counter using the same structure as shown in Figure 1. (PRELAB)

2. Annotate all Q outputs of your schematic with the bit of the counter (Q7Q6Q5Q4Q3Q2Q1Q0) that they correspond to (where Q7 is the most significant bit and Q0 is the least significant bit. Label the inputs according to the diagram in Figure 1. (PRELAB)

3. Build the circuit corresponding to your schematic. Your circuit should use the flip-flop module provided by Logisim, instantiated eight times to create the counter. (PRELAB)

Note that for the modules that you are instantiating, it is best if you use the default input and output from the toolbar. It is recommended that you should name your inputs and outputs in a way that makes it easy to interpret your simulations (e.g. use input/output names from your schematic).

4. Connect the Q output bits to two seven-segment displays so you can monitor the output values. (PRELAB)

5. Test your modules with Poke( ) to verify its correctness. You will need to reset (clear) all your flip-flops early in your simulation, to ensure that your circuit starts in a known state. Include screenshots of simulation output in your prelab. (PRELAB)

5 Part II

Another way to specify an counter would be to instantiate a register and finding a way to add 1 to the register value every time the clock goes high. Adding 1 can be accomplished using the Adder under Arithmetic. The constant value 1 can be found in Wiring &gt; Constant, where the value and the number of data bits for this constant can be set in Properties after you click on it.

5.1 The Counter Device

Figure 2: Counter in Logisim

Figure 2 shows an example of a counter in Logisim that counts in hexadecimal from 0 to F. You can find this counter in Memory &gt; Counter.

The counter has the following input signals:

1. An active-high asynchronous clear (R at the top left corner),

2. Signals M1 [load] and M2 [count] that perform load and counter enable. An input of 1 makes the counter load a new multi-bit value (provided in the bottom left of the device) and 0 tells the counter to start counting up or down.

3. The signals M3 [up] and M4 [down] (note that they are just one signal) determine whether to count up or down.

4. The inputs called 2,3,5+/C6 and 2,3,5+/C6 should be connected to a Clock signal.

5. The four-bit inputs on the bottom left of the counter take in the value to load into the counter (when the load bit M1 is high) and the value that the counter stores can be seen on the output wires on the bottom right side of the counter.

The implementation above is a 4-bit counter, however you can change this in Properties if you wish to use more bits. In your prelab report, provide the answers to the following questions:

1. The check for the maximum value is not necessary in the example above. Explain why in your prelab report. (PRELAB)

2. If you wanted this 4-bit counter to count from 0-9, how would you adjust the circuit above? (PRELAB)

3. In Properties there is a setting called Action On Overflow. Explain how each value for this setting responds to overflow by experimenting with this setting and describing the results. (PRELAB)

5.2 The Rate Divider and the Display Counter

In this part of the lab you will design and implement a circuit using counters that successively flashes the hexadecimal digits 0 through F on a hex display. A two-bit input value to your circuit will be used to determine the speed of flashing according to the following table:

SW[1] SW[0] Speed

0 0 Full (32 Hz)

0 1 1 Hz

1 0 0.5 Hz

1 1 0.25 Hz

You must design a fully synchronous circuit, which means that every flip flop and/or counter in your circuit should be clocked by a 32Hz clock signal, provided by Logisim. You will then use a counter to generate the slower clock signals outlined by the table above.

This is different from setting the speed of the simulation clock in Logisim. For this lab we want to assume that your circuit is taking in a clock signal that is fixed at a fast speed and your circuit needs to dynamically slow it down based on the SW[1] and SW[0] inputs. For instance, if we were uploading our designs onto the DE1-SOC boards, the built-in clock on that board runs much faster, at 50 MHz (50,000,000 times per second). You need to demonstrate that you can create circuitry that could handle this 50MHz task by slowing down a 32Hz signal instead.

The output of the circuit you create will be a new clock signal that is used for the hex display to make its digits flash at the speed indicated by SW[1] and SW[0] in the table above, assuming that you’re starting with the 32Hz clock provided by Logisim during your simulation.

Two modules are required to make this happen:

1. A special kind of counter called a RateDivider which takes in the 32Hz clock signal and outputs a new clock signal, slowed down to a rate specified by SW[1] and SW[0].

2. A second counter called DisplayCounter. This is a hexadecimal counter that is responsible for counting through the values 0 – F. Recall that an enable signal determines whether a flip flop, register, or counter will change on an active edge of the clock or not.

The output of the RateDivider generates a slower alternating signal, which is then used as the enable signal of the DisplayCounter module. Every time RateDivider has counted the appropriate number of clock edges, it generates a high output pulse for one clock cycle. For example, Figure 3 shows a timing diagram that produces a 1 Hz pulse signal from a 50 MHz clock (the kind used on the DE1-SOC board). The resulting 1 Hz pulse signal would provide the Enable value for the DisplayCounter module.

In your prelab report, calculate how large a counter would be required to count 50 million clock cycles, as illustrated by Figure 3. How many binary bits would that counter need to represent such a value? (PRELAB)

Figure 3: Timing diagram for a 1 Hz enable signal

A common way to count a specified number of clock pulses is to load a starting value into the RateDivider counter then have the counter count down to zero. For example, if you want to count one second given a 50MHz clock (as in the DE1-SoC example), you can load the RateDivider counter with a value of 50 million and subtract one at each time the clock pulses until the counter reaches 0 (strictly speaking, you would load the value 49,999,999). Once a 50MHz counter has counted down from 50 million, one second has passed and the DisplayCounter can be incremented by one. Then the RateDivider counter would then reload the starting value again.

A few more notes about your final circuit:

1. The AND gate on the right side of Figure 2 performs two tasks: it turns on the output Enable signal once the counter reaches a certain value and it performs a parallel load of a new counter value (specified by you) on the next clock cycle. This is one way to make the RateDivider counts a certain number of clock cycles before turning on the enable signal (but not the only one). Using this idea, changing the frequency of the new clock signal would just involve changing the value you load into the counter.

• This counter design in Figure 2 is provided for you and you can use it as a model to build your RateDivider counter (your DisplayCounter will be more straightforward).

• You don’t have to follow this model exactly. As long as you use the counter provided by Logisim, you can use whatever other circuitry you prefer to implement the RateDivider behaviour. Be creative! We only provide this idea to get you thinking about what your circuit needs to do.

2. DisplayCounter counts 4-bit binary values, incrementing each time its Enable input is 1. When the counter reaches 1111, the next increment should reset it to 0000. The output of this DisplayCounter should be directed to a seven-segment display so that the TAs can observe the counter result. • You can use whichever counter you’d prefer for this part, either the one you created in Part I or Logisim’s built-in counter.

5.3 What you need to do

For this part of the lab, you need perform the following steps (in addition to answering the questions labeled as PRELAB in the sections above):

1. Draw a schematic of the circuit you wish to build. In particular, show how the outputs of the RateDivider feed into the inputs of the DisplayCounter, and how the high-level inputs and outputs connect to your entire circuit. Mentally step through the usage of this circuit to ensure that your circuit handles the necessary use cases to the best of your understanding. (PRELAB)

2. Build the circuit that realizes the behaviour described in your schematic. Your main circuit should have one clock input, one reset input and two external switch inputs (SW[1] and SW[0]) for the RateDivider. The circuit should have a seven-segment display as output. (PRELAB)

HINT: You should name the inputs and outputs of each module in a way that makes it easy to interpret your simulations (e.g. use input/output names from your schematic).

3. Simulate your modules with Poke( ). Choose test cases that make you feel confident about your counter’s correctness in preparation for you in-lab demo. Make sure to include a few selected screenshots of these cases when you hand in your prelab. You will also need to think about the best way to simulate this kind of circuit. For example, how many 32 Hz clock pulses will you need to simulate to show that the RateDivider is properly outputting a 1 Hz pulse? (PRELAB)

(HINT: Sometimes simulating a circuit in its entirety is infeasible. It is therefore important to identify which are the critical aspects of the circuit you need to simulate to be confident that your circuit will work. Demonstrating this for a smaller problem can be one valid approach.)

4. Label your high-level Logisim design with the appropriate input and output names that would be used on the DE1-SoC board (e.g. use HEX0 as the seven-segment display from the DisplayCounter while using switches SW1−0 to control the rate at which these hex digits are updated). You will also need to use additional switches (e.g., the clear signal). (PRELAB)

6 Part III

In this part of the lab you are going to design and implement a Morse code encoder.

Morse code uses patterns of short and long pulses to represent a message. Each letter is represented as a sequence of dots (a short pulse), and dashes (a long pulse). For example, the last 8 letters of the English alphabet have the following representation:

S • • •

T —

U • • — V • • • —

W • — — X — • • — Y — • — —

Z — — • •

Your circuit should take as input one of the eight letters of the alphabet shown in the table above. The output will be an LED that flashes the dots and dashes that that display the Morse code signals for that letter (you can find LEDs in Input/Output &gt; LED).

To make this happen, you need to create the following:

1. A lookup table (LUT) to store the Morse code sequences for each letter,

2. A shift register to display the Morse signals,

3. A rate divider to set the timing for the shift register.

6.1 Displaying Morse Code Signals

Let us first look into how we will store the Morse code representation for each letter. A ”dot” will cause the LED to flash for 0.5 seconds while a ”dash” will cause the LED to flash for 1.5 seconds. Since both of these times are multiples of 0.5 seconds, we will use this to our advantage when representing a Morse code sequence as a sequence of binary numbers.

Each Morse code sequence will be a sequence of 1s and 0s where the 1 indicates when the LED should turn on and the 0 indicates when the LED will turn off. Let’s assume that each bit corresponds to a display duration of 0.5 seconds, so a single 1 bit in the sequence will correspond to a ”dot” (the LED should stay on for 0.5 seconds), while three 1s in a row (i.e., 111) will correspond to a ”dash” (the LED should stay on for 3∗0.5 seconds). The sequence will then use 0 values to separate those signals (i.e., the LED will turn off for 0.5 seconds in between dots and dashes). As a result, the LED could be off either during a pause (e.g., a transition between a Morse dash and a dot), the beginning/end of a transmission, or if there is no transmission.

6.2 The Lookup Table (LUT)

Using this representation, the Morse code for letter X could be stored as 1110101011100000, assuming we use 16-bits to represent it (this is not a required length). Every letter from S to Z will have a binary sequence like this that represents the on/off sequence on the output LED. So we need a device that takes in the letter to display and outputs this binary sequence. This is a kind of decoder called a Lookup Table (LUT).

To implement the LUT, you’ll want to fill in the remaining entries in Table 1 with the Morse code binary representation that would display the remaining 7 letters (S to Z). (PRELAB)

• Note that each letter will require a different minimal number of bits in this representation. However, you will need to make sure all the sequences are the same length because they all need to be loaded into a single shift register to display them on the LED. The shift register will be a fixed length, therefore the length of your binary sequences below will also need to be a single fixed length. • To figure out what this length will be, you need to figure out the maximum number of bits needed when representing the Morse code sequences for each of the letters (S to Z). Once you have that, adjust all of the binary sequences to match that maximum length. For letters that do not require that maximum number of bits, extend any of the 0 sections of that sequence. Make sure that the last bit of any Morse code representation is set to 0.

Fill in Table 1 below as part of your prelab. You will need to fill in the header of the third column with the sequence length you decided on. You will also need to pad the sequence for letter X with added zeroes as needed to match the sequence length you chose. (PRELAB)

The LUT device will store the binary representation of each Morse code pattern and use a multiplexer to determine which pattern is sent to the output bits. Since there are 8 letters to display, the LUT will take in a 3-bit input to specify the letter, where 000 denotes the sequence for letter S and 111 denotes the sequence for letter Z. So if each Morse sequence was 16 bits long, the LUT would have a 3-bit input and a 16-bit output. This LUT is asynchronous, so no clock or reset signals are needed.

6.3 The Shift Register and the Rate Divider

The next module to consider is the shift register. If the LUT is supplying a sequence of on/off signals to display on the LED, we need a module that can display each bit, one at a time. In order to do that, we

Letter Morse Code Pattern Representation (sequence length is bits)

S • • •

T —

U • • —

V • • • —

W • — —

X — • • — 111010101110

Y — • — —

Z — — • •

Table 1: Morse Pattern Representation with fixed bit-width (PRELAB)

can use a shift register by following these steps:

1. Load the sequence from the LUT into the shift register (using the shift register’s parallel load). Make sure the shift register length is the same as the sequence length from Table 1.

2. Shift the sequence by one bit each time the clock goes high.

3. Have the bit that is shifted out of the register displayed on the LED.

The third and final module that you will need is the rate divider, which will supply the shift register with the appropriate clock signal (one that goes high every 0.5 seconds).

A high-level block diagram of the circuit you are building is shown in Figure 4. Note that various details/connections are not shown there.

Figure 4: Block diagram of the Morse code circuit

To summarize, once the user presses a button that starts the LED display process you need to load a shift register with the appropriate pattern (for the letter specified by a 3-bit input) and display the Morse code from that pattern on the LED. Note that you should not display a given letter in a loop (i.e., you should only re-display the same letter if the user presses the start button again).

6.4 What you need to do

Complete the lab by performing the following steps:

1. Use Table 1 to determine your codes and bit-width. (PRELAB)

2. Design your circuit by first drawing a schematic of the circuit. Think about and work through your schematic to make sure that it will work according to your understanding. You can use Figure 4 as your starting point. You should include the schematic in your prelab. (PRELAB)

3. Build the circuit in Logisim that realizes the behaviour described in your schematic. (PRELAB)

HINT: You should name your inputs and outputs in a way that makes it easy to interpret your simulations (e.g. use input/output names from your schematic).

4. Simulate your LUT with test vectors and your shifter module with Poke( ). Choose test cases that make you feel confident about your LUT and shifter’s correctness in preparation for your in-lab demo. You are strongly encouraged to complete this step before performing your lab demo. Document the test cases that you considered (especially the corner cases) in your prelab report and include screenshots of the most interesting cases. (PRELAB)

5. Label the inputs and outputs of your Logisim design to correspond to the inputs and outputs on the DE1-SoC board. The following table summarizes the inputs and outputs that you will use:

(PRELAB)

Input/Output Purpose

SW[2:0] Choose one of the 8 letters S to Z

KEY[1] Start diplaying Morse code for chosen letter

KEY[0] Asynchronous reset

LEDR[0] Output used to display Morse code
