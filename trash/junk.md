* Task Summary

Remove call_email-address() from the *Business Parameters* configuration via the Oracle BPM Process Adminstrator console.

* Implementation Plan
** Step 1. Login to Oracle BPM Process Adminstrator console

| Console URL      | http://askdjfhkasd:10006/webconsole/ |
| Console Username | adlklasd                             |
| Console Password | alkdfadjksfk                         |
#+TBLFM: @1$2='(org-sbe obpm-pa-url () )::@2$2='(org-sbe obpm-pa-username () )::@3$2='(org-sbe obpm-pa-password () )

*Note:* Use Chrome or Microsoft IE because Safari may not display correctly.

** Step 2. Navigate to *Business Parameters* configuration screen

1. Click plus =[+]= icon next to =Organization= on left-hand side of screen to expand tree.

2. Click =Business Parameters= item.

   - The screen will refresh but this may take a few minutes.

3. Click black left triangle icon

   - The screen will refresh and two new buttons will be displayed on the left-hand side of screen.

4. Click =Filter= link on left-hand side of screen.

   - The screen will refresh and a new filter form will be displayed.

5. Click left form field then choose =Organization Value= from drop-down menu.

6. Click middle form field then choose =Contains= from drop-down menu.

7. Click right form field and enter call_email-address().

8. Click =Apply= button.

   - The screen will refresh and display =Business Parameters= configurations which contain call_email-address().

9. Copy all text from filtered table into a text file and add to ticket as a reference in case of rollback. 

For example, the following was copied from production on <2015-03-25 Wed>
#+BEGIN_EXAMPLE
	Name	Type	Organization Value
	ABO_TECHNICAL_EXCEPTION_EMAIL	String	asdjkoasjdfjasld
	CCR_TECHNICAL_EXCEPTION_EMAIL	String	asdfasdfasdfas
#+END_EXAMPLE
 
** Step 3. Remove call_email-address() from the =Organization Value= of each business variable.

1. Click the link of top item listed in the =Name= column.

2. Remove call_email-address() from =Organization Value= including commas (,) as needed.

3. Click =Save= Button.

4. Repeat above steps until filtered table is empty. 
