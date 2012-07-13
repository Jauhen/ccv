CCV Input Plugin
================

Description
===========

This is a CCV input plugin for the jQuery javascript library.

It allows input card number with masking and hidding first digits.

Plugin supports next bank card numbers:
- Master Card (mc)
- Visa/Visa Electron (visa)
- American Express (amax)
- Diner's Club (dc)
- China UnionPay (cup)

Change Log
==========

Version 0.1.0
- Initial version.

Examle of ussage
================

Source code of sampe usage

    <script type="text/javascript" src="http://code.jquery.com/jquery-1.4.2.js"></script>
    <script type="text/javascript" src="http://jquery-joshbush.googlecode.com/files/jquery.maskedinput-1.2.2.js"></script>
    <script type="text/javascript" src="ccv.js"></script>
    <script type="text/javascript">

     $(document).ready(function(){
         $("#a").ccv($.ccv.cup);
     });

    </script>
    <form method=get>
        <input id="a" type="text" name="a" value="" class="text"><br/>
        <input type="button" onclick="$('#a').newccv($.ccv.mc);" value="Master Card">
        <input type="button" onclick="$('#a').newccv($.ccv.visa);" value="Visa">
        <input type="button" onclick="$('#a').newccv($.ccv.amex);" value="AMEX">
        <input type="button" onclick="$('#a').newccv($.ccv.dc);" value="Diner's Club">
        <input type="button" onclick="$('#a').newccv($.ccv.cup);" value="UnionPay">
        <input type=submit> 
    </form>

Credits
=======

Plugin has been created by Yauhen Kutsuk (jauhen@gmail.com)

It needs Masked Input Plugin to run.

Also some ideas from iphone-password have been used.

Licensed as MIT
===============

    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
    furnished to do so, subject to the following conditions:

    The above copyright notice and this permission notice shall be included in
    all copies or substantial portions of the Software.
    
    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
    THE SOFTWARE.