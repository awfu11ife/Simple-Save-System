# Simple-Save-System
This system allows you to save any type of data in Player Prefs
Simple Save System allows you to easily save any type of data to Player Prefs by converting it to JSON. To use it:
 1) Place the DataPersistencer.cs script on an empty object in the scene.
 2) Create a class with a public field/fields of the data type(s) you want to save, inherit it from the DataToSave class, and create a parameterless constructor that sets default values for the fields.
 3) Implement the IDataPersistence interface in the script where you want to save something.
An implementation example can be found in the Example folder.
Please note that DataPersistencer.cs automatically saves and loads data only for the classes that are included at the scene's launch. If you want to save data manually, simply execute the Save and Load methods anywhere in the class that implements the interface.
