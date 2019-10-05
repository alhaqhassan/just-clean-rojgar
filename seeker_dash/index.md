---
layout: seeker_dash
title: job seekers
description: just no description.
theme_color: grey
---
<div class="pages" id="home">
home
</div>
<div class="pages" id="add_job_form">
    <div>
    <form id="add_job_form_html">
    <input type="hidden" name="job_id" id="job_id">
        <div class="row">
            <div class="col s10 input-field ">
                <input id="job_title" name="job_title" type="text" class="validate">
                <label for="job_title">Job Title</label>
            </div>
            <div>
                <input type="submit" class="btn grey" value="post">
            </div>
            <div class="col l8 s12 input-field ">
                <input id="job_description" name="job_description" type="text" class="validate">
                <label for="job_description">Job Description</label>
            </div>
            <div class="col s12 l4 input-field ">
                <select id="job_profile" name="job_profile">
                    <option value="" disabled selected>Job Profile</option>
                </select>
            </div>
            <div class="col s12 l4 input-field ">
                <select name="job_creteria">
                    <option value="" disabled selected>Job creteria</option>
                    <option value="Class 5th to 9th">Class 5th to 9th</option>
                    <option value="10th Pass">10th Pass</option>
                    <option value="12th Pass">12th Pass</option>
                    <option value="Polytechnic">Polytechnic</option>
                    <option value="Diploma">Diploma</option>
                    <option value="Graduate(B.A.,B.Com.,B.Sc">Graduate(B.A.,B.Com.,B.Sc)</option>
                    <option value="Other Graduate(Any Stream)">Other Graduate(Any Stream)</option>
                    <option value="B.Tech(Any Stream)">B.Tech(Any Stream)</option>
                    <option value="M.Tech(Any Stream)">M.Tech(Any Stream)</option>
                    <option value="Post Greaduate(Any Stream)">Post Greaduate(Any Stream)</option>
                    <option value="MBA/PGDM(Any Stream)">MBA/PGDM(Any Stream)</option>
                </select>
            </div>
            <div class="col s12 l4 input-field ">
                <select name="job_experience">
                    <option value="" disabled selected>Experience</option>
                    <option value="Experience (0 to 1 yrs)">Experience (0 to 1 yrs)</option>
                    <option value="Experience (1 to 2 yrs)">Experience (1 to 2 yrs)</option>
                    <option value="Experience (2 to 3 yrs)">Experience (2 to 3 yrs)</option>
                    <option value="Experience (3 to 4 yrs)">Experience (3 to 4 yrs)</option>
                    <option value="Experience (above 5 yrs)">Experience (above 5 yrs)</option>
                </select>
            </div>
            <div class="col s12 l4 input-field ">
            <input type="text" class="datepicker" placeholder="last_date" value="Last Date For Apply">
            </div>
        </div>
        <div>
        </div>
        </form>
    </div>
</div>
<div class="pages" id="post_now_job">
    <div>
    <div class="row">
        <div class="col s8">
            <h4>Jobs: <a href="#!add_job_form" class="btn grey">New</a></h4>
        </div>
        <!-- <div class="col s2">
            <div class="col s12 input-field ">
                <input id="q" type="text" class="validate">
                <label for="q">Search</label>
            </div>
        </div> -->
        </div>
        <ul id="employer_job_lists" class="collection">
            <li class="collection-item">            
                <div class="row">
                    <div class="col s6"><a href="#!">Title</a></div>
                    <div class="col s4">Description</div>
                    <div class="col s2"><a href="#!">Delete</a></div>
                </div>
            </li>
        </ul>
    </div>
</div>
<div class="pages" id="seekers_applied">
ddddddddd
</div>
<style>
    /* .collection li a{padding:15px!important} */
    .collection div{margin:0!important}
</style>
<script>
var job_profile_list=["Machine Operator / Helper","IT / ITeS","Driver (Private Vehicles)","Driver (Commercial Vehicles)","Driver (Heavy Vehicles - Bus, Truck, etc.)","Bouncer","Security Staff","Security Guard","Security Guard (Armed)","PSO (Personal Security Officer)","Computer Operator","Data Entry Operator","Plumber","Electrician","Housekeeping Staff","Retail Sales Staff","Retail Store Keeper","Cashier","Sales Manager","Field Officer","Supervisor","Beautician","BPO / Call Centre","Receptionist","Management / Admin","HR","Accounts Executive","GST Executive","ESIC / PF Executive","Cook","Tailor","Delivery Jobs","Carpenter","Painter","Mason","Construction Worker","Bar Binder","Welder","CNC machine operator","Fitter","Domestic Help / Maid / Home-cleaning","Rider","AC Repairing / AC Service","Electronics Repair","Home Appliances Repair","Waiter (Restaurant)","Bartender","Hair Dresser (Male)","Hair Dresser (Female)","Personal Assistant","Peon","DG Operator","STP Operator","WTP Operator","Lift Operator","Lift Technician","Water Tank Cleaner","Car Washer / Cleaner","Web Designer","Web Developer","Graphic Designer","Fitness Trainer","Yoga Trainer","Logistics Staff (Loading / Unloading )","Packaging Staff","Warehouse Staff","Nursing Staff","Patient Care","Baby Sitter / Nanny / Mother Care","Parking Management Staff","MST (Multi Tasking Staff)","Housekeeping Supervisor","Security Supervisor","Training Supervisor","Landscaping supervisor","Plumbing Supervisor","Manpower Mobiliser","Leather Worker","Dairy Worker","Façade Cleaner","Band-Baaja Staff","Party Singers","Others",]
	for(i=0;i<job_profile_list.length;i++){
		var option = document.createElement("option");
		option.text = job_profile_list[i];
		option.value = job_profile_list[i];
		var select = _("job_profile");
		select.appendChild(option);
	}
</script>