Please find debugging options in Developer Debug Mode > Inpaint:

- Debug Enhance Masks: outputs generated masks, default disabled
- Debug GroundingDINO: early return in the detection process, uses GroundingDINO boxes instead of refined SAM detections inside those boxes. This option can sometimes improve results when SAM isn't able to correctly detect inside GroundingDINO boxes. FYI: GroundingDINO supports detection prompts, SAM auto-detects objects without further promps inside of the boxes.
- GroundingDINO Box Erode or Dilate: increase/decrease the detected box area by GroundingDINO. This option can sometimes improve SAM detection when GroundingDINO accidentally cuts off elements (very rare)

|                                                                                                                                                                                                                                                                            |
| :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|                                                                                            \|GroundingDINO\|                                        \|GroundingDINO + SAM\|<br>                                                                                            |
| ![image](https://github.com/user-attachments/assets/897ca491-6af2-4a08-b32b-52655514c765)\|[![image](https://github.com/user-attachments/assets/469319c4-544f-42f6-96f0-e34ea10cedd2)](https://github.com/user-attachments/assets/469319c4-544f-42f6-96f0-e34ea10cedd2)\|] |
