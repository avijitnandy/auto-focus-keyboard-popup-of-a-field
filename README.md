# auto-focus-keyboard-popup-of-a-field
How to remove auto focus/keyboard popup of a field when the screen shows up?

I found two perfect way to do that.
1. Programmatic way:

InputMethodManager imm = (InputMethodManager)getSystemService(Context.INPUT_METHOD_SERVICE);
imm.hideSoftInputFromWindow(editTextField.getWindowToken(), 0);

2. By setting activity property in manifest file as below
 
 android:windowSoftInputMode="stateHidden"
