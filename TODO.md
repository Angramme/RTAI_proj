
## Tips from tutorial
- Read the README, imporant stuff such as:
    - Note that all inputs are images with pixel values between 0 and 1. The same range also applies to all abstract bounds that we want to verify.
- Implementation:
    - Think about batch dimension in dimensions and shapes
    - Dont get screwed on that, always be aware of the shape sizes
    - the +cpu in the versions sometimes bugs and does not want to install
- Myybe install TQDM locally (instead of Matplotlib)
- _**We do not need branch and bound**_, use DeepPoly ReLU Relaxations instead (look at slides)
- Think about how to find good slopes
    - should be done in one to two loops
    - also first write the project without the optimal slopes
- Think where and how to find intermediate bounds
- Represent the data well as to not get lost in the implementation
- Think about all cases of the activation functions
- Try the DLN networks (which dont have activation functions) to test basic stuff out
    - DeePoly is exact on those networks
- Use a very small network for debugging, (for example the network from the slides)
    - also make it a bit longer because a lot of issues arise when there is more layers