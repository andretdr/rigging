# Rigging fundementals   
### Keep objects clean   
- delete history   
- freeze transformation *sets* all values to zero   
- center pivot
- scale and rotate joints is fine, *dont* translate
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
- Rigging -> Skeleton -> Mirror Joints Options (Mirror Behavior for rotation correctness)
- curves -> Rebuild (increasing spans on curve)
- deform -> nonlinear -> bend
- animation -> key -> set driven key

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
- Mode: Select, dbl click vertex to select affected object
- Mode: Paint, value 01, Flood. Object should turn white
- Go to next object

## Bendy Surface Skinning
- create joints
- bind skin
- Animate the extreme deformation on the joints and paint accordingly


# Controls
- create similar heirachy from controls to joints
- Ctrls should have a group where you can have values, but yr curve should be clean.
- orientate yr ctrl groups to be exact to joints
- you can edit or change yr curve/ctrl CVs to create interesting shapes, but the curve orientation shouldnt change
- Use nonlinear deform bend for more interesting shapes

## Set Driven Keys
animation -> keys -> set driven keys
- select driver joint -> load driver -> select driving attribute
- select driven joints -> load driven -> driven attr(s)
- key (Now you've set the first keypose between the driving and driven)
- create your next key pose (diver then driven)¡¡™¡ and hit key


MUSCLE SYSTEM
https://80.lv/articles/chris-jones-flexes-digital-muscles-in-a-new-mind-blowing-demo/

