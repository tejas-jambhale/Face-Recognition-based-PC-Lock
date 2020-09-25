## One Day Build

### Simple app to lock your pc when accessed by someone else.


### Create Training set
Run train.py to create the unlock data set. Take pictures of your face to keep the screen unlocked

`
py train.py data/train/0 2000
`

Similarly run train.py again to create lock set. Add random faces, objects for which the screen should get locked

`
py train.py data/train/1 2000
`

### Validation dataset also needs to be added
Repeat as above for

`
py train.py data/valid/0 200
`
`
py train.py data/valid/1 2000
`

### Run the code
first run model.py
`
py model.py
`
then to begin tracking
`
py predict.py
`

Remember the program will be active as long as 'q' is not pressed. Until then webcam will remain on




