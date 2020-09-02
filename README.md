# Strange-Python-Code
I find the else clause on loop constructs to be quite weird. Here is a piece of code taken from the source code of wtforms. It illustrates a typical use case.
data = self.data 
if data is not None: 
 for pk, obj in self._get_object_list(): 
  if data == obj: 
   break 
 else: 
  raise ValidationError(self.gettext('Not a valid choice')) 
