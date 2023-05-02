# trax
research notebooks with Trax framework

[01_trax_intro_nlp.ipynb](01_trax_intro_nlp.ipynb)
- introduction notebook to Trax

[02_classes_inheritance.ipynb](02_classes_inheritance.ipynb)
- about classes, subclasses and inheritance
- `__init__` function and `__call__` function

### Gradient Descent in Trax
![image](https://user-images.githubusercontent.com/49360095/235598463-45cf74fa-1f1f-45b2-8a47-a5dfa13cfc03.png)
Now if you were to evaluate grad_f at a certain value, namely z, it would be the same as computing 6z+1.  Now to do the training, it becomes very simple: 
![Screenshot from 2023-05-02 13-16-17](https://user-images.githubusercontent.com/49360095/235598283-c2603df5-0893-4d80-ac47-d04346f4948e.png)

You simply compute the gradients by feeding in y.forward (the latest value of y), the weights, and the input x, and then it does the back-propagation for you in a single line. You can then have the loop that allows you to update the weights (i.e. gradient descent!).
