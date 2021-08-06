## A visit to your doctor's:
%% Adapted from A Smarter Way to Learn Python  (Meyers, n.d.) %%

On your first visit to a health clinic, the receptionist hands you a clipboard with a form to fill out.
You fill out the form to provide your personal information. 

Why a form? Why not just a blank sheet of paper with instructions "Tell us about yourself"?

The clinic wants a *standard set of information organized the same way for each* patient.
The form is a template that makes things easier for both you and the clinic.
	It standardizes and organizes information so that the information is easier to access and work with.
	
> In Python, [[class | classes]] are templates. They help you standardize and organize information.

The receptionist's tablet of forms is like a [[class]].
	Before it's filled out, each sheet in the folder is identical to all the others.
	When a patient fills out a copy, it still has the same structure as all the others but it also contains unique particulars to each individual patient.
	
In other words, each patient will have their own [[instance]] of this form, but the information for all patients will be structured the same way.

```py
class Patient():
	...
```

When you write this line, what you're really saying is:
"I'm creating a class that I'm naming **Patient**."
Use this class as the template for each virtual sheet of information on a patient.

