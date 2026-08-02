---
date: 2026-02-27
---


This is a summary from Release notes (https://wiki.freecad.org/Release_notes_1.0). With FreeCAD 1.0.0 being released as stable, I read through the news and want to share with you what I found useful for creating models for 3d printing.

I've been already using it for a bit, it's all great. Big thanks to everyone who contributed.

# more straightforward UI

Many tools have been unified into more universal modifications which choose variants automatically based on context. It's more pleasant and faster to use.

Measuring distance, lengths, angles etc. is now done by std measure (https://wiki.freecad.org/Std_Measure). It has auto mode which computes what you need based on what you select.

Analogously, constraining distances and alike in Sketcher has been merged into one tool called dimensions (https://wiki.freecad.org/Sketcher_Workbench#Sketcher_CompDimensionTools), which again is context sensitive. It's interactive and let's you decide if there are more alternatives. The same goes for horizontal/vertical constraints.

All coincidence and pointOnObject constraints are joint into a single constraint.

Among other changes to UI: when creating an object, parameters of such (like height or angle) are displayed in real time. You can also just type a number and hit enter to choose manually.

Rectangles and slots have now more mods and can create broader category of shapes. Also, chamfers and fillets are more powerful in Sketcher now.

Lastly, you can create offsets (https://wiki.freecad.org/Sketcher_Offset). When you create offset, another curve is created surrounding the selected one with a fixed distance. It also works inside.
# entity manipulation

Tools have been added to manipulate objects. Notably, in the Part WorkBench you can scale and mirror Parts. No need to switch into the Draft WB.

The same for Sketcher, you can scale, rotate, transform, create arrays, work with symmetry. Also, simple copy-paste works and it's python code copied, so you can copy-paste between sketchers and even files (or even share it on a forum!).

Also, you can remove all constraints from a sketch to the axes, which allows you to drag the object freely. This combined with the copy tools from the previous paragraphs makes up a strong combination.

The transform tool dragger now not only supports dragging in a line, but in plane too.

# topo naming problem mitigation

It's not fully mitigated (as that's not possible), but you can now reference parts of 3d objects, like faces and it should work. This is particularly nice in combination with padding a face or padding up to a shape (not just a face as before).

# small things

You can pad (or otherwise work with) only a part of a sketch, simply select it.

Part design allows (experimental opt-in) multiple solids in a body.

New tool (https://wiki.freecad.org/Std_AlignToSelection) for aligning view with a selected face has been added.
# TODO for me

There's new Assembly WB which I know nothing of, it's next on my todo list. Also, FEM WB might be cool to look into to inspect weak points of models before printing them.

As you can see, a lot of fun awaits. Can't wait to model more in FreeCAD.