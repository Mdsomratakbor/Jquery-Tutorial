# JQuery change() Event 
`The change event is sent to an element when its value changes. This event is limited to <input> elements, <textarea> boxes and <select> elements. For select boxes, checkboxes, and radio buttons, the event is fired immediately when the user makes a selection with the mouse, but for the other element types the event is deferred until the element loses focus.`

<div class="col-md-12">
            <div class="card">
                <div class="card-header">
                    <h3>JQuery Change() and mouserover() Event</h3>
                </div>
                <div class="card-body">
                    <table class="table">
                        <tbody><tr>
                            <td>First Name</td>
                            <td>
                                <input id="txtFirstName" type="text" class="inputRequired">
                            </td>
                            <td>
                                <img id="imgFirstNameHelp" src="images/unnamed.png" width="30" height="30" style="cursor: pointer;">
                            </td>
                            <td>
                                <div id="divFirstNameHelp" style="display: none;">First Name as show in passport</div>
                            </td>
                        </tr>
                        <tr>
                            <td>Last Name</td>
                            <td>
                                <input id="txtLastName" type="text" class="inputRequired">
                            </td>
                            <td>
                                <img id="imgLastNameHelp" src="images/unnamed.png" width="30" height="30" style="cursor: pointer;">
                            </td>
                            <td>
                                <div id="divLastNameHelp" style="display: none;">Last Name as show in passport</div>
                            </td>
                        </tr>
                        <tr>
                            <td>City</td>
                            <td>
                                <select id="ddlCity" class="inputRequired">
                                    <option value="Select">Select</option>
                                    <option value="New York">New York</option>
                                    <option value="London">London</option>
                                    <option value="Chennai">Chennai</option>
                                    <option value="Sydney">Sydney</option>
                                </select>
                            </td>
                            <td><img id="imgCityHelp" src="images/unnamed.png" width="30" height="30" style="cursor: pointer;"></td>
                            <td>
                                <div id="divCityHelp" style="display: none;">
                                    Your residence city</div>
                            </td>
                        </tr>
                        <tr>
                            <td>Favourite Color</td>
                            <td>
                                <input id="radioRed" name="color" type="radio" value="Red" class="inputRequired">Red
                                <input id="radioGreen" name="color" type="radio" value="Green" class="inputRequired">Green
                                <input id="radioBlue" name="color" type="radio" value="Blue" class="inputRequired">Blue
                            </td>
                            <td><img id="imgColorHelp" src="images/unnamed.png" width="30" height="30" style="cursor: pointer;"></td>
                            <td>
                                <div id="divColorHelp" style="display: none;">
                                    Your Favourite Color</div>
                            </td>
                        </tr>
                        <tr>
                            <td>Contact Method</td>
                            <td>
                                <input id="chkBoxEmail" type="checkbox" value="Email" class="inputRequired">Email
                                <input id="chkBoxPhone" type="checkbox" value="Phone" class="inputRequired">Phone
                                <input id="chkBoxSocialMedia" type="checkbox" value="Social Media" class="inputRequired">Social Media
                            </td>
                            <td><img id="imgContactMethodHelp" src="images/unnamed.png" width="30" height="30" style="cursor: pointer;"></td>
                            <td>
                                <div id="divContactMethodHelp" style="display:none">
                                    How should we contact you</div>
                            </td>
                        </tr>
                        <tr>
                            <td>
                                Comments
                            </td>
                            <td>
                                <textarea id="txtComments" class="inputRequired"></textarea>
                            </td>
                            <td><img id="imgCommentsHelp" src="images/unnamed.png" width="30" height="30" style="cursor: pointer;"></td>
                            <td>
                                <div id="divCommentsHelp" style="display:none">
                                    Your comments please</div>
                            </td>
                        </tr>
                        <tr>
                            <td>
                                <button class="btn btn-sm btn-success" id="each">Submit</button>
                            </td>
                            <td>
                                <div id="divResult"></div>
                            </td>
                        </tr>
                    </tbody></table>
                    <div id="result">    
                    </div>
                    <div id="result2">
                    </div>
                </div>
                <div class="card-footer">
                    <button class="btn btn-sm btn-success" id="each">Submit</button>
                </div>
            </div>
        </div>
