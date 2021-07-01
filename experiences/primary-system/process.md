# Primary system

The Primary system includes at minimum 5 blocks.

- 1 Outside interface
- Direct memory
- Decision system
- 1 System-i
- Outside

To simplify the study, I will implement a living being that lives in a 1D world.

Quickly, you will figure out that there is something inherent in every form of life. This is energy. So I have to keep track of the energy of the living being and to give it a way of getting back energy.

The Outside will be a line that goes from right to left with one energy source at a time.

The Outside interface will be a sensor that position of the energy source relative to the position of the living being.

The Direct memory will be a linear function.

The Decision system will be a threshold function.

The System-i will give the ability to the living being to move left or right.

The Direct memory has 3 variables. One for the the Outside interface, one for a bias and one for the loop.

The Decision system has 2 variables. The first one is the threshold to go left, the second one to go right. If the value is between the two, the living being don't move.

The living being has a maximum level on energy. Each movement use a part of this energy. The energy slowly decays over time.

That adds up to 7 variables that describes the living being.

There won't be any learning process, the living being simulated here will be as simple as possible. However, I need a way of making evolved the living being. The easier way is to use reproduction and generation.

Each living being can reproduce (there is no concept of sex for now). After reproduction, the living being die and it's divided into 4 living being. Each children have variables similar to their parents.

Reproduction cost energy.

Finally, each living being is described by 8 variables.
