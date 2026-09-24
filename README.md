# Ex7-Animator-Movement

### Name - R SUDHIR KUMAR
### Register number - 212223230221

## Aim :

To develop a animator movement for a player using unity.

## Algorithm :

## Step 1 : 

Import necessary models.

## Step 2 : 

 Right-click -> Create -> Animator Controller.

## Step 3 : 

Open Animator window, define states (Idle, Run, Jump, etc.).

## Step 4 : 

Use keyframes or Unity's Animation tools to animate transitions between states.

## Step 5 : 

Drag Animator Controller to the GameObject in the Inspector.

## Program :

### DEVELOPED BY : Ashwin Kumar A
### REG NO : 212223040021
PlayerController:


```
using System.Collections;
using System.Collections.Generic;
using UnityEngine;

public class Movement : MonoBehaviour
{
    public Animator animator;
    public float InputX;
    public float InputY;
    // Start is called before the first frame update
    void Start()
    {
        animator=this.gameObject.GetComponent<Animator>();
        
    }

    // Update is called once per frame
    void Update()
    {
        InputX = Input.GetAxis("Horizontal");
        InputY = Input.GetAxis("Vertical");
        animator.SetFloat("InputX", InputX);
        animator.SetFloat("InputY", InputY);
        
    }
}

```
## Output :

<img width="1917" height="1078" alt="Screenshot 2026-09-01 144908" src="https://github.com/user-attachments/assets/b1728310-2d24-4bd3-ba28-e717c67e97d7" />

## Result :

An animator movement for a player using unity is developed successfully.
