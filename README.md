# Ring3-Rootkit-Remover-Renamed



Unhooks all ring 3 rootkits, and specifically removes the stock r77 rootkit installation.

# Requirements
You need to run the remover as admin.
# Todo
- [ ] Gui
- [X] Update weekly
- [X] Rename
# Suggestions
Please tell me if you have any suggestions
# RAT payload looking for Ring3 and other things
```csharp
private static bool smethod_1(ref int int_0, ref int int_1, ref int int_2, ref StringBuilder stringBuilder_0, ref string string_0, ref string[] string_1, ref int int_3, ref string string_2, IntPtr intptr_1)
	{
		StringBuilder stringBuilder = new StringBuilder(256);
		stringBuilder_0 = stringBuilder;
		GClass14.GetWindowText(intptr_1, stringBuilder_0, 256);
		string[] array = new string[] { "Removal Tool", "Removal_Tool", "SeroXen Removal Tool", "SeroXen_Removal_Tool", "Unhooker", "Ring3" };
		string text = stringBuilder_0.ToString();
		string_0 = text;
		string[] array2 = array;
		string_1 = array2;
		int_3 = 0;
		int_0 = 56;
		return false;
	}
```
