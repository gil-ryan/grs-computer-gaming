# Player-v-Player Macro

## Targeting

### Arena

### Basics

```macros
/target arena1
/target arena2
/target arena3
```

## Mage

### Non-Spec

#### Polymorph

Set and announce Polymorph

```macro
/clearfocus
/focus
/stopmacro [help]
/clearfocus
/stopmacro [noexist] [dead]
/focus
/run SetRaidTarget("focus",0);
/run SetRaidTarget("focus",5);
/e is targeting %t for Polymorph.
Polymorph the set target
#showtooltip Polymorph
/stopcasting
/Use [combat] Presence of Mind
/Use [@focus] Polymorph
```
