# World of Warcraft Macros

## Index

* UI
    + Frames

## fstack

When __fstack__  is enabled, hovering over different frames will 
give you detailed information about them.

![fstack while hovering over PlayerFrame](https://github.com/gil-ryan/grs-computer-gaming/blob/master/BLIZZARD/world-of-warcraft/img/fstack.PNG)

```macro
/fstack
```

## Player Frame

Default __Frame__ size is _i_.

![PlayerFrame](https://github.com/gil-ryan/grs-computer-gaming/blob/master/BLIZZARD/world-of-warcraft/img/playerframe.PNG)

### Set PlayerFrame Larger

```macro
/run PlayerFrame:SetScale(2)
```

### Default PlayerFrame

```macro
/run PlayerFrame:SetScale(1)
```

### Set TargetFrame 

```macro
/run TargetFrame:SetScale(2)
```

### Hide Frame

You can disable a __Frame__ with the following commands. Using the _Hide()_ macro will disable the __Frame__ Entirely, and you no longer be able to interact with it.

```macro
/run PlayerFrame:Hide()
/run TargetFrame:Hide()
```

You can hide a __Frambe__ but still interact with it using _SetAlpha()_. Changing the parameter in _SetAlpha()_ will effect it's transparency.

```macro
/run PlayerFrame:SetAlpha(0)
```

### Sample Macro

```macro
/run PlayerFrame:SetScale(1.15)
/run TargetFrame:SetScale(1.15)
/run FocusFrame:SetScale(1.15)
/run PartMemberFrame1:SetScale(1.15)
/run PartyMemberFrame2:SetScale(1.15)
/run PartyMemberFrame3:SetScale(1.15)
```

## Bars and Menus

### Adjust location on UI

```macro
/run CharacterMicroButton:ClearAllPoints()
/run CharacterMicroButton:SetPoint("CENTER", -709, -745)
/run CharacterMicroButton:SetPoint = function() end
```
