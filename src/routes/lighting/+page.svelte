<script>
	import lightoff from './lightoff.png';
	import lighton from './lighton.png';
	import powerButton from './PowerButton.png';
	import powerButtonOn from './PowerButtonOn.png';

	let powerOn = false;
</script>

<div class="light-control">
	<div class="slider-container">
		<!-- <input type="range" class="slider" id="myRange" min="1" max="100" value="50">
        <div>Value: <span id="demo"> <input type="text" placeholder="test"></span></div> -->
		<div class="slider-value-div">
			<input
				class="slider-value"
				id="example-value"
				type="number"
				max="100"
				min="0"
				value="50"
				step="1"
				source="[name=example]"
			/>
		</div>
		<img class="slider-image" src={lightoff} />
		<input class="slider" name="example" type="range" max="100" min="0" value="50" step="1" />
		<img class="slider-image" src={lighton} />
	</div>
	<div class="light-buttons">
		<div class="timer-button">
			<button onclick="myFunction()" class="dropbtn">Timer</button>
			<div id="myDropdown" class="dropdown-timer">
				<a href="#"
					>Hours
					<select>
						<option value="0">0</option>
						<option value="1">1</option>
						<option value="2">2</option>
						<option value="3">3</option>
						<option value="4">4</option>
						<option value="5">5</option>
						<option value="6">6</option>
						<option value="7">7</option>
						<option value="8">8</option>
						<option value="9">9</option>
						<option value="10">10</option>
						<option value="11">11</option>
						<option value="12">12</option>
						<option value="13">13</option>
						<option value="14">14</option>
						<option value="15">15</option>
						<option value="16">16</option>
						<option value="17">17</option>
						<option value="18">18</option>
						<option value="19">19</option>
						<option value="20">20</option>
						<option value="21">21</option>
						<option value="22">22</option>
						<option value="23">23</option>
						<option value="24">24</option>
					</select>
				</a>
				<a href="#"
					>Minutes
					<select>
						<option value="0">0</option>
						<option value="1">1</option>
						<option value="2">2</option>
						<option value="3">3</option>
						<option value="4">4</option>
						<option value="5">5</option>
						<option value="6">6</option>
						<option value="7">7</option>
						<option value="8">8</option>
						<option value="9">9</option>
						<option value="10">10</option>
						<option value="11">11</option>
						<option value="12">12</option>
						<option value="13">13</option>
						<option value="14">14</option>
						<option value="15">15</option>
						<option value="16">16</option>
						<option value="17">17</option>
						<option value="18">18</option>
						<option value="19">19</option>
						<option value="20">20</option>
						<option value="21">21</option>
						<option value="22">22</option>
						<option value="23">23</option>
						<option value="24">24</option>
						<option value="25">25</option>
						<option value="26">26</option>
						<option value="27">27</option>
						<option value="28">28</option>
						<option value="29">29</option>
						<option value="30">30</option>
						<option value="31">31</option>
						<option value="32">32</option>
						<option value="33">33</option>
						<option value="34">34</option>
						<option value="35">35</option>
						<option value="36">36</option>
						<option value="37">37</option>
						<option value="38">38</option>
						<option value="39">39</option>
						<option value="40">40</option>
						<option value="41">41</option>
						<option value="42">42</option>
						<option value="43">43</option>
						<option value="44">44</option>
						<option value="45">45</option>
						<option value="46">46</option>
						<option value="47">47</option>
						<option value="48">48</option>
						<option value="49">49</option>
						<option value="50">50</option>
						<option value="51">51</option>
						<option value="52">52</option>
						<option value="53">53</option>
						<option value="54">54</option>
						<option value="55">55</option>
						<option value="56">56</option>
						<option value="57">57</option>
						<option value="58">58</option>
						<option value="59">59</option>
						<option value="60">60</option>
					</select>
				</a>
				<button onclick="closeTimer()" class="timer-set"> Set </button>
			</div>
		</div>

		<button style="background: none; border:none;">
			<img class="power-button" src={powerOn ? powerButtonOn : powerButton} />
			<!--Power Button -->
		</button>
		<div class="schedule-button">
			<button onclick="openSchedule()" class="dropsch">Schedule</button>
			<div id="scheduleDropdown" class="dropdown-schedule">
				<input type="time" />
				<span style="margin-left: 5px; margin-right: 5px">to</span>
				<input type="time" />
				<button onclick="closeSchedule()" class="schedule-set"> Set </button>
			</div>
		</div>
	</div>
</div>
