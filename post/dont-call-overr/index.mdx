---
title: "Don't call overridable methods in constructors"
date: "2007-10-04"
categories: 
  - "software-development"
tags: 
  - "eclipse"
excerpt: 'MS has a rule about this in'
---

MS has a rule about this in [FxCop](external:https://msdn2.microsoft.com/en-us/library/ms182331\(VS.80\).aspx). PMD has a rule:

##### [ConstructorCallsOverridableMethod](external:https://pmd.sourceforge.net/rules/design.html). In both cases the point is to discourage the following weird behaviour. From Eclipse:

```
public abstract class CellEditor {
    protected CellEditor(Composite parent, int style) {
        this.style = style;
	System.out.println("CellEditor constructor");
        create(parent);
    }
```

public void create(Composite parent) {         Assert.isTrue(control == null);         control = createControl(parent);    }     protected abstract Control createControl(Composite parent) }

.....

```
public class HyperlinkCellEditor extends TextCellEditor {
	public HyperlinkCellEditor(Composite parent, int style, otherParams) {
		super(parent, style);
		System.out.println("HyperlinkCellEditor constructor")
	}
```

protected Control createControl(Composite parent) {             System.out.println("createControl");     return newly created control;       } }

When run the output of this code is:

```
CellEditor constructor
createControl
HyperlinkCellEditor constructor
```

Sadly this means createControl (which you must implement) doesn't have access to local variables (they're not yet initialized) nor does it have access to HyperlinkCellEditor's other params. Now we have to initialize our control in two parts. The generic part is done in the createControl and the part specific to our data in the constructor. Its bad enough that they called an overridable method from the constructor. Far worse that they made it abstract. I wasted a chunk of time trying to debug this mess a few days.

To the eclipse guys: come on not even MS would allow this to be checked into the .NET framework. Who thought this was a good idea?

Sorry for the lack of posts in the last week a perfect storm of events has conspired to keep me busy.

Next up a post on the [perils of protected variables](/blog/protected-varia) - which stunningly Eclipse also uses.
