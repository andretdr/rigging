# Rigging fundementals   
### Keep objects clean   
- delete history   
- freeze transformation *sets* all values to zero   
- center pivot
- 
### Idea
- Geom moved by joints by skinning
- Joints moved by controllers by constraints

## Hot keys   
#### d   
pivot mode
#### v
snap mode
#### p
select child, then parent, hit p
#### shift - p
unparent child

## Setting up shelf   
- create new shelf   
- ctrl + shift + click on menu item to add to shelf   

## Important Tools   
- Delete by type history   
- Delete by type nondeformer history   
- Modify -> Freeze transform   
- Modify -> Center Pivot   
- Rigging -> Display -> Transform Display -> View Local Rotation Axis (Show *joints* and *Handles*)   

## Joints
- Tools settings   
![image](https://github.com/user-attachments/assets/005e2c11-bd6d-49eb-917b-bc54feaae7ad)
- Be careful of where the joints are pointing, turn on local rotation axis to see   
- Joint Orient on attr editor. When you freeze joints, their joint orientation remains   
- You can scale and rotate joints, do NOT translate joints. Freeze after   
- scale the radius on attr if too big   

# Skinning
## Hard Surface Skinning
- create all your joints   
- select all joints, select geom   
- rigging -> skin -> bind -> bind to: selected joints    
![image](https://github.com/user-attachments/assets/17daeedc-3b2d-4d19-b562-3450f6bcda2e)

- Select Geom
- rigging -> skin -> paint skin weights (make sure use color ramp is on)
![image](https://github.com/user-attachments/assets/11c9040f-fdcf-4068-a715-28fd603f707e)

- Start from tips and go inwards
- Identify joint
- Mode: Select
- Dbl click vertex to select affected object
- Mode: Paint
- Value 01, Flood. Object should turn white
- Go to next object

- 
