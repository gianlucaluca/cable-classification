# Cable Classification

This project uses the Jetson Nano to tell the difference between common household cables such as USB, HDMI, and USB-C to show the different appearances of each cable.
Their naming does not provide much benefit to the user, so this program can tell the difference for you.

## The Algorithm

This program uses image classification to detect which type of USB cable is in the image frame. Using resnet18 as the base model, the machine gives its best estimate to which type of USB cable is in frame.

## Running this project

1. SSH into nano (through your preferred means)
2. Run the command `./docker_dli_run.sh` to enter into the jupyter labs docker
3. Write down the link and password given to you (should look like an ip address, with :8888 or such)
4. Run `cd classification`
5. Run `wget https://github.com/gianlucaluca/cable-classification/blob/master/cableclassification.ipynb`
6. Run `cd ..` to get back to the original directory
7. Run `cd data/classification`
8. Run `wget https://github.com/gianlucaluca/cable-classification/blob/master/cablemodel.pth`
9. On another machine, use the previous link to login into JupyterLabs 
10. Click the classification folder
11. click on the `cableclassification.ipynb` file
12. [Click the two arrows at the top of the screen](https://i.imgur.com/j1BchcY.png)
13. [Once the display opens, go to the file path area and type `/nvdli-nano/data/classification/final_project.pth`](https://i.imgur.com/T0BFU2i.png)
14. Click load model
15. make sure 'state' is live
16. If not working, try clicking evaluate

## Video

[Video Explanation](https://youtu.be/8AT4mmfRHiw)
