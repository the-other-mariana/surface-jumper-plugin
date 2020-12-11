<p align="center">
  <img width="600" height="450" src="https://github.com/the-other-mariana/surface-jumper-plugin/blob/master/render/ad-gif.gif">
</p>
<br />

# Surface Jumper Plugin

This plugin takes an object and makes it jump over a series of control points that you add by clicking on any editable poly you have on a 3dsMax Scene. <br />

## Specifications

Version of 3dsMax: `Autodesk 3dsMax 2020`

## Getting Started

1. Download [test scene](https://github.com/the-other-mariana/surface-jumper-plugin/blob/master/test-scene-raycast.max) and [script](https://github.com/the-other-mariana/surface-jumper-plugin/blob/master/surface-jumper.ms). <br />

2. Open test scene from step 1. <br />

3. In 3dsMax, go to `Scripting > MAXScript Editor > Open File`. Open the script from step 1. <br />

4. Click anywhere over the editor. <br />

5. Type `Ctrl + A` and then `Ctrl + E` to open the plugin window. <br />

## Usage

### Prepare Params 

1. On Surface Jumper window, click on `Select Jumper`. <br />

2. On max scene, select the teapot in the scene by clicking on it. To check you have a jumper, the button should now display the object's name. <br />

3. On Surface Jumper window, click on `Add Point`. <br />

4. On max scene, click on any surface to put a control point. A small black circle will appear on the surface you clicked. <br />

5. Make a right click. <br />

6. Repeat steps 3 to 5 in order to add more jump control points. You must have more than 2 points. When you finish placing points, continue on next section. <br />

### Customize Each Jump

7. On Surface Jumper window, in `Jump Params` section, select the `Interpolation Style` you want: `Physical` is face-normal based (looks better in curved surfaces) or `Biased` (looks good in horizontal surfaces). <br />

8. On Surface Jumper window, `Frames Per Jump` is the amount of frames in the time line that each jump will take. Default set to 24, but click on the arrows of the spinner to add or substract frames. <br />

9. On Surface Jumper window, `Roll Angle` is the angle that the jumper will spin when jumping. Default set to 90, but click on the arrows of the spinner to add or substract angle. <br />

### Customize The Jump Sequence

10. On Surface Jumper window, in `Jump Sequence Params` section, select the `Jump Strength` style you want. `Decay`, for example, makes the jump sequence decrease its strength each jump. It's how the height of each jump will be handled. <br />

11. On Surface Jumper window, `Strength Value` the strength or height you want for all jumps. Default set to 15, but click on the arrows of the spinner to add or substract strength. <br />

12. On Surface Jumper window, `Squash Frames` is the amount of frames you want to use from each jump's frames to squash the object when it touches the floor. Default set to 5, but click on the arrows of the spinner to add or substract strength. Do not exceed half the amount of `Frames Per Jump`. <br />

13. On Surface Jumper window, `Squash Limit` is a slider where you will choose the maximum squash value. <br />

14. On Surface Jumper window, `Constant Squash` checkbox is where you choose if the amount of squash per jump is according to the height (unchecked) or constant (checked). <br />

15. Click on `Create Jumps` button to apply everything and generate the sequence. <br />

*Note: You may want to have your time line include some negative frames so that you see the anticipation to the jumps.* <br />

## Example

The plugin window should look something like this: <br />

![alt text](https://github.com/the-other-mariana/surface-jumper-plugin/blob/master/images/window.png?raw=true) <br />

An example of the usage and result is below. <br />

![alt text](https://github.com/the-other-mariana/surface-jumper-plugin/blob/master/images/example-gif.gif)<br />
