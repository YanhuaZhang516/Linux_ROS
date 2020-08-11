# tf_ros tutorial
## 1. what is tf (Transform Frames)?

Thanks to TF, we can add sensors and parts to the robot, and the TF will handle all the relations for us. 
**tf broadcaster** is used to publish the coordinate frames and a **tf listener** is used to compute the difference in the different frames and move to another.
If we want to know the position of the object related to base_link, the only thing we need to do is call TF library and get the transformation.

## 2. tf tools

### 1. writing a tf broadcaster

how to broadcast the state of a robot to tf. 

#### 1. create package

#### 2. how to broadcast transforms
#### 3. running the broadcaster
#### 4. checking the results

### 2. Writing a tf listener

how to use tf to get access to frame transformation

### 3. Adding a frame

how to add an extra fixed frame to tf

### 4. learning about tf and time

how to use the `waitForTransform` function to wait for a transform to be availabe on the tf tree.

### 5. Time travel with tf

