# CppChecklist
A small checklist for a normal day's code review.

<h3>Includes</h3>
<ul>
<li>Proper include guard is added</li>
<li>No duplicate includes</li>
<li>Proper include format: 
 <ul>
<li>No relative/absolute paths</li>
<li><> for library and system includes</li>
<li>"" for user-defined type includes</li>
</ul>
</li>
<li>Check proper order</li>
</ul>

<h3>Classes</h3>
<ul>
<li>Rule of Three: One exists, Create all.
<ul>
<li>Destructor</li>
<li>Copy constructor <b>class_name(const class_name &)</b></li>
<li>Copy assignment operator <b>operator=(const class_name &)</b></li>
</ul>
</li>
<li>Use initializer list for user defined type for better performance</li>
<li>Check proper const-ness of functions/parameters/members</li>
<li>Private default constructors for static classes</li>
</ul>

<h3>Variables/Access</h3>
<ul>
<li>Check variable/parameter initialization</li>
<li>Check that pointers are initialized</li>
<li>Check pointers (for nullptr value) before use.</li>
<li>Create reference variables as necessary</li>
<li>No hardcoded numbers.</li>
</ul>

<h3>General Scope</h3>
<ul>
<li>Use for(auto& element : elements) for STL containers</li>
<li>Check if typdef/using alias is applicable</li>
</ul>
