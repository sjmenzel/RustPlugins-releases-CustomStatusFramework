Still WIP, do not review.

# API
``` csharp
void CreateStatus(string text, string subText, string color, string imageLibraryIconId, Func<BasePlayer, bool> condition);

void CreateDynamicStatus(string text, string color, string imageLibaryIconId, Func<BasePlayer, bool> condition, Func<BasePlayer, string> dynamicValue);
```