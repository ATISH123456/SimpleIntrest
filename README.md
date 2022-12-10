public ActionResult SimpleInterest()  
{  
    return View();  
}  


<h2>Calculate Simple Interest</h2>  
<fieldset>  
        <legend>Calculate Simple Interest</legend>  
    @using (Ajax.BeginForm("CalculateSimpleInterestResult","CalculateSimpleInterest",  
                            new AjaxOptions { UpdateTargetId = "divInterestDeatils" }))  
    {  
        <div id="divInterestDeatils"></div>  
        <ol>  
            <li>  
                @Html.Label("Amount")  
                @Html.TextBox("txtAmount")  
            </li>  
            <li>  
                @Html.Label("Rate")  
                @Html.TextBox("txtRate")  
            </li>  
            <li>  
                @Html.Label("Year")  
                @Html.TextBox("txtYear")  
            </li>  
        </ol>  
    <button>Calculate</button>  
    }     
</fieldset>  
