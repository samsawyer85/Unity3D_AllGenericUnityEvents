# Unity3D_AllGenericUnityEvents

According to Unity's Manual if you want to make your own UnityEvent utilizing a custom signature you need to declare a new class like so:

```
[Serializable]
public class StringEvent : UnityEvent <string> {}
```

It supports up to 4 arguments of any combination of String, Float, Int, Bool, and Object.
With that in mind, not wanting to declare a new class each time I needed a custom event, I made this class that has every combination of those 5 types, from 1 to 4 arguments.

Not a complicated script at all, but it's convenient to have and easy to use:

```
using UnityEngine;
using System.Collections;

public class CustomEventExample : MonoBehaviour 
{
    public UnityEvents.F myFloatEvent;
    public UnityEvents.BI myBoolIntEvent;

    // Use this for initialization
    void Start () {

    }

    // Update is called once per frame
    void Update () {

    }
}
```

![CustomEventExample Inpsector](http://i.imgur.com/aProeag.png "CustomEventExample Inpsector")
