<p><strong><u>Major Business Requirements:</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong>Ritchie Feed &amp; Seed Inc</strong>. started as a supplier and now it is flourished in retail garden business having various branches in the city. On these branches there are number of employes working on different roles.</p>
<p>These business offers various kind services such as selling retail products, arranging different workshops, and providing green team services which can cover entire gardening from initial stage to maintain the plants all in one for the customer. The retail items import from the company&rsquo;s warehouses through their own transportation. Customer can direct contact with the company based on their requirements through user inquiry form which allows them to resolve their all queries related to gardening. To fulfill the customer&rsquo;s requirements company have record about the product&rsquo;s stock at each branch and warehouses. Customer can place an order as a single material as well as in bulk and that order can be prepared by one or many employees.&nbsp; This order bill can count the total revenue for the business.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>Assumptions:</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p>&nbsp;</p>
<ul>
<li>We assumed that the &lsquo;<strong>Ritchie&rsquo;s Green Team&rsquo;</strong> is the sub part of the main business, in which they provide various services rather than actual products. so, their employees are subject maters experts due to that reason we added flag (EmployeeOfGreenTeamFlag) to differentiate in the employee table.</li>
</ul>
<p>&nbsp;</p>
<ul>
<li>The administrative team who receives user inquiry form can easily<strong> bifurcate the inquiry form is for Ritchie&rsquo;s Green Team or for General Business </strong>so, we put a Flag (FlagMsgForGreenTeam).</li>
</ul>
<p>&nbsp;</p>
<ul>
<li>User inquiry form can be access by <strong>registered customers or any website visitors</strong>.</li>
</ul>
<p>&nbsp;</p>
<ul>
<li>The main business of this company as a supplier so, we assumed that they have their <strong>own transportation</strong>.</li>
</ul>
<p>&nbsp;</p>
<ul>
<li>We added DeliveryTime in Order entity because as per our assumption customer can <strong>place an online order or purchase on store as well</strong>.</li>
</ul>
<p>&nbsp;</p>
<ul>
<li>We assumed that <strong>one order from customer can be prepared by one or many employees</strong> at a time, so that is why we joined order entity to employee entity.</li>
</ul>
<p><strong>&nbsp;</strong></p>
<ul>
<li>This is the retail and supply business that is why we assumed that they need to take <strong>records of each product&rsquo;s stock</strong>.</li>
</ul>
<p>&nbsp;</p>
<ul>
<li>Customer can order more than one item at a time so it is not necessary to store OrderID, OrderDate, DeliveryTime, TotalPrice and PaymentMethod in every ordered product so, we created separate table to store all ordered products and linked it with order entity with OrderID which can <strong>reduce the data repetition</strong>.</li>
</ul>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>ERD:</u></strong></p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>Relational Schema:</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p>&nbsp;</p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<p><strong><u>Lessons Learned:</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<ul>
<li>This exercise helps to think from customer point of view so we learned to make design which is user understandable form as they may not be the subject mater experts of IT field.</li>
<li>Make sure to put relevant attributes in the entities which can helps to reduce data repetition.</li>
<li>We learned to think out of the box to cover business and imagine other requirements because every time it is not possible that client cover all the topics, so we as a designer must think other relevant things. For example<strong>, the main business is as a supplier so, they need transportation</strong>.</li>
<li>Understand the granularity of the business and accordingly make that level of granule design.</li>
</ul>
<p>&nbsp;</p>
<p><strong><u>What you would do differently:</u></strong></p>
<p><strong><u>&nbsp;</u></strong></p>
<ul>
<li>There are some limitations for this assignment such as resources, time, knowledge. But if we get more resources and time with proper business guidance then we would like to cover some important sides of the company such as we tried to make &lsquo;<strong>Hiring Procedure&rsquo;</strong> of this company.</li>
</ul>
<p>&nbsp;</p>
<ul>
<li>Every business has <strong>some Policies</strong> but here we do not have any information about it so, can not cover that part in design.</li>
<li>Ritchie Feed &amp; Seed Inc. is a big organization so they are using some resources and pay for it as well as they take products from other organizations, but lack of our knowledge about it we are unable to create such design of it, so if we get proper information about it then we can design accordingly, and they can <strong>manage and observe their revenue and cost.</strong></li>
</ul>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><strong><u>References:</u></strong></p>
<p><strong>&nbsp;</strong></p>
<p><a href="https://www.ritchiefeed.com/">https://www.ritchiefeed.com/</a>&nbsp;</p>
<p><a href="https://www.tutorialspoint.com/dbms/er_model_basic_concepts.htm">https://www.tutorialspoint.com/dbms/er_model_basic_concepts.htm</a></p>
<p>&nbsp;</p>
