# EntityLogger

Open solution, build CecilTest, plop Assembly-CSharp.dll in the bin folder,
run CecilTest, copy Assembly-CSharp.out.dll over Assembly-CSharp in the
Hearthstone_Data/Managed folder it came from.  Mark as read-only for less pain
with Battle.net client.  Copy HookRegistry.dll and Newtonsoft.Json.dll to the
Managed folder as well.  See results in entity.log in Hearthstone's root folder.

Newtonsoft.JSON is compiled specially for Unity, involves removing anything
dependent on System.Data.  Dependencies not included in the lib folder are
binaries from Hearthstone's Hearthstone_Data/Managed folder.