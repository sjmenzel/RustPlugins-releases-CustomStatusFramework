Still WIP, do not review.

# Developer API
``` csharp
void CreateStatus(
  string text, 
  string subText, 
  string color, 
  string imageLibraryIconId, 
  Func<BasePlayer, bool> condition
);

void CreateDynamicStatus(
  string text, 
  string color, 
  string imageLibaryIconId, 
  Func<BasePlayer, bool> condition, 
  Func<BasePlayer, string> dynamicValue
);
```

# Code Examples

``` charp
Func<BasePlayer, bool> condition = (basePlayer) => { return basePlayer.secondsConnected < 60; };
CustomStatusFramework.Call("CreateStatus", "New Player", "Welcome!", "0.3 0.6 0.9 1", "img_id_here", condition);
```