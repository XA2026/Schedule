<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Ximena &amp; Andy's Wedding Week · August 22–30, 2026</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=EB+Garamond:ital,wght@0,400;0,500;1,400&family=Pinyon+Script&family=Poppins:wght@300;400;500;600&display=swap" rel="stylesheet">
<style>
  :root{
    --paper:#FAF4CE;
    --paper-deep:#F5EDBE;
    --green:#24503A;
    --green-soft:#4A6B54;
    --gold:#A97C2C;
    --rose:#A15C4E;
    --sage:#7F8768;
    --ink:#33372E;
    --muted:#71755F;
    --dot:rgba(36,80,58,.28);
    --script:"Pinyon Script","Snell Roundhand",cursive;
    --serif:"EB Garamond",Garamond,Georgia,serif;
    --sans:"Poppins","Avenir Next",system-ui,sans-serif;
  }
  *{box-sizing:border-box;}
  html,body{margin:0;padding:0;}
  body{
    background:var(--paper);
    color:var(--ink);
    font-family:var(--sans);
    font-weight:300;
    -webkit-font-smoothing:antialiased;
    -webkit-print-color-adjust:exact;
    print-color-adjust:exact;
  }
  .sheet{max-width:1240px;margin:0 auto;padding:44px 44px 0;}

  /* ---------- header ---------- */
  header{text-align:center;}
  .who-line{font-size:11px;letter-spacing:.44em;text-transform:uppercase;color:var(--green);font-weight:500;}
  header h1{font-family:var(--script);font-size:60px;font-weight:400;color:var(--gold);line-height:1.04;margin:12px 0 8px;}
  header .dates{font-family:var(--serif);font-style:italic;font-size:18px;color:var(--green-soft);}

  /* ---------- filter bar ---------- */
  .bar{
    position:sticky;top:0;z-index:20;background:var(--paper);
    padding:16px 0 14px;margin-top:26px;
    border-top:1px dotted var(--dot);border-bottom:1px dotted var(--dot);
    text-align:center;
  }
  .set{display:inline-flex;flex-wrap:wrap;justify-content:center;gap:6px;}
  .set + .set{margin-top:10px;}
  .btn{
    font-family:var(--sans);font-size:10.5px;letter-spacing:.24em;text-transform:uppercase;
    font-weight:500;color:var(--muted);background:none;border:1px solid transparent;
    padding:8px 16px;cursor:pointer;transition:all .18s ease;
  }
  .btn:hover{color:var(--green);}
  .btn[aria-pressed="true"]{color:var(--green);border-color:rgba(36,80,58,.4);background:rgba(36,80,58,.05);}
  .btn:focus-visible{outline:2px solid var(--gold);outline-offset:2px;}
  .set.loc .btn{font-size:9.5px;letter-spacing:.2em;padding:6px 13px;color:var(--muted);}
  .legend{display:flex;flex-wrap:wrap;justify-content:center;gap:8px 22px;margin-top:14px;}
  .legend span{display:flex;align-items:center;gap:7px;font-size:9px;letter-spacing:.18em;text-transform:uppercase;color:var(--muted);}
  .legend i{width:14px;height:3px;display:inline-block;}
  .i-bride{background:var(--gold);} .i-family{background:var(--green);}
  .i-guest{background:var(--rose);} .i-rest{background:var(--sage);}

  /* ---------- sections ---------- */
  section.band{margin-top:52px;}
  .band-head{display:flex;align-items:center;gap:16px;margin-bottom:26px;}
  .band-head h2{
    font-size:11px;letter-spacing:.36em;text-transform:uppercase;color:var(--green);
    font-weight:600;margin:0;white-space:nowrap;
  }
  .band-head .loc{font-family:var(--serif);font-style:italic;font-size:15px;color:var(--muted);}
  .band-head::after{content:"";flex:1;border-top:1px dotted var(--dot);}

  .row{display:grid;gap:0;}
  .r4{grid-template-columns:repeat(4,1fr);}
  .r2{grid-template-columns:repeat(2,1fr);}
  .r3{grid-template-columns:1fr 1.16fr 1fr;}
  .dayc{padding:0 26px 30px;border-left:1px dotted var(--dot);}
  .row .dayc:first-child{padding-left:0;border-left:none;}

  /* ---------- day heading ---------- */
  .dayname{font-family:var(--script);font-size:38px;font-weight:400;color:var(--green);line-height:1;margin:0;}
  .daydate{font-size:11px;letter-spacing:.24em;text-transform:uppercase;color:var(--gold);font-weight:500;margin-top:10px;}
  .daytag{font-family:var(--serif);font-style:italic;font-size:14.5px;color:var(--green-soft);margin-top:10px;line-height:1.4;}

  /* ---------- person groups ---------- */
  .group{margin-top:24px;}
  .who{
    font-size:9.5px;letter-spacing:.26em;text-transform:uppercase;font-weight:600;
    color:var(--green);padding-bottom:6px;margin-bottom:14px;border-bottom:1px dotted var(--dot);
  }
  .who.g{color:var(--rose);}
  .who.a{color:var(--green-soft);}
  .group[hidden]{display:none;}

  .item{margin-bottom:16px;padding-left:13px;border-left:3px solid var(--sage);}
  .item:last-child{margin-bottom:0;}
  .b-bride{border-left-color:var(--gold);} .b-family{border-left-color:var(--green);}
  .b-guest{border-left-color:var(--rose);} .b-rest{border-left-color:var(--sage);}
  .t{font-family:var(--serif);font-size:14.5px;color:var(--ink);letter-spacing:.03em;margin-bottom:3px;}
  .t .ap{font-size:11px;letter-spacing:.08em;}
  .a{font-size:15px;font-weight:600;color:var(--ink);line-height:1.3;}
  .c{font-size:12.5px;font-weight:300;color:var(--muted);line-height:1.5;margin-top:3px;}
  .p{font-size:12.5px;color:var(--green-soft);margin-top:2px;}
  .mini{font-size:9px;letter-spacing:.2em;text-transform:uppercase;color:var(--gold);font-weight:500;margin-top:7px;}

  .note{margin-top:20px;padding:11px 13px;border:1px solid rgba(169,124,44,.35);background:rgba(169,124,44,.07);}
  .note b{display:block;font-size:9px;letter-spacing:.24em;text-transform:uppercase;color:var(--gold);font-weight:600;margin-bottom:4px;}
  .note span{font-size:12.5px;color:var(--ink);font-weight:400;line-height:1.45;}

  .tiny{margin-top:18px;padding-top:12px;border-top:1px dotted var(--dot);}
  .tiny b{display:block;font-size:8.5px;letter-spacing:.24em;text-transform:uppercase;color:var(--green);font-weight:600;margin-bottom:4px;}
  .tiny span{font-size:11.5px;color:var(--muted);line-height:1.55;font-weight:300;}

  .empty{font-family:var(--serif);font-style:italic;font-size:14px;color:var(--muted);margin-top:24px;}

  /* ---------- footer ---------- */
  footer{margin:64px 0 0;padding:30px 0 46px;border-top:1px dotted var(--dot);text-align:center;}
  footer .k{font-size:10px;letter-spacing:.36em;text-transform:uppercase;color:var(--green);font-weight:600;}
  .protect{display:flex;flex-wrap:wrap;justify-content:center;gap:10px 30px;margin-top:20px;}
  .protect div{font-size:11.5px;color:var(--muted);font-weight:300;}
  .protect em{font-style:normal;font-weight:600;color:var(--gold);letter-spacing:.14em;text-transform:uppercase;font-size:9.5px;margin-right:7px;}
  footer p{font-family:var(--script);font-size:32px;color:var(--gold);margin:30px 0 0;}

  @media (max-width:1000px){
    .r4{grid-template-columns:repeat(2,1fr);}
    .r3{grid-template-columns:repeat(2,1fr);}
    .dayc{padding:0 20px 28px;}
    .r4 .dayc:nth-child(2n+1),.r3 .dayc:nth-child(2n+1){padding-left:0;border-left:none;}
    .r4 .dayc:nth-child(n+3),.r3 .dayc:nth-child(n+3){padding-top:30px;}
  }
  @media (max-width:720px){
    .sheet{padding:26px 18px 0;}
    header h1{font-size:40px;}
    .r4,.r2,.r3{grid-template-columns:1fr;}
    .dayc{padding:0 0 26px;border-left:none;border-top:1px dotted var(--dot);padding-top:26px;}
    .row .dayc:first-child{border-top:none;padding-top:0;}
    .r4 .dayc:nth-child(n+3),.r3 .dayc:nth-child(n+3){padding-top:26px;}
    .dayname{font-size:34px;}
    .bar{padding:12px 0 10px;}
  }
  @media (prefers-reduced-motion:reduce){*{transition:none!important;}}
  @media print{
    .bar{position:static;}
    body{background:#fff;}
    .dayc{break-inside:avoid;}
    section.band{break-inside:avoid;}
  }
</style>
</head>
<body>
<div class="sheet">

  <header>
    <div class="who-line">Gloria + Antonio</div>
    <h1>Ximena &amp; Andy&rsquo;s Wedding Week</h1>
    <div class="dates">August 22&ndash;30, 2026 &middot; Washington, DC &amp; New York City</div>
  </header>

  <div class="bar">
    <div class="set" id="whoSet">
      <button class="btn" data-who="everyone" aria-pressed="true">Everyone</button>
      <button class="btn" data-who="gloria" aria-pressed="false">Gloria</button>
      <button class="btn" data-who="antonio" aria-pressed="false">Antonio</button>
    </div>
    <div class="set loc" id="locSet">
      <button class="btn" data-loc="all" aria-pressed="true">All</button>
      <button class="btn" data-loc="dc" aria-pressed="false">DC</button>
      <button class="btn" data-loc="nyc" aria-pressed="false">NYC</button>
    </div>
    <div class="legend">
      <span><i class="i-bride"></i>Ximena &amp; wedding</span>
      <span><i class="i-family"></i>Pascuala &amp; family</span>
      <span><i class="i-guest"></i>Guests &amp; friends</span>
      <span><i class="i-rest"></i>Rest &amp; protected</span>
    </div>
  </div>

  <!-- ============ DC ============ -->
  <section class="band" data-loc="dc">
    <div class="band-head">
      <h2>DC &middot; Family Days</h2>
      <span class="loc">August 22&ndash;25</span>
    </div>

    <div class="row r4">
      <!-- SAT -->
      <div class="dayc">
        <h3 class="dayname">Saturday</h3>
        <div class="daydate">August 22</div>
        <div class="daytag">Arrival. Nothing more.</div>

        <div class="group" data-who="gloria">
          <div class="who g">Gloria</div>
          <div class="item b-family">
            <div class="t">Afternoon</div>
            <div class="a">Pascuala + America Arrive</div>
            <div class="c">Settle in &middot; unpack &middot; slow.</div>
          </div>
        </div>

        <div class="group" data-who="both">
          <div class="who">Gloria + Antonio</div>
          <div class="item b-family">
            <div class="t">Evening</div>
            <div class="a">Dinner at Home</div>
            <div class="c">Immediate family only.</div>
          </div>
          <div class="item b-rest">
            <div class="t">Night</div>
            <div class="a">Rest</div>
          </div>
        </div>

        <div class="tiny"><b>Arriving</b><span>Pascuala &middot; America</span></div>
        <div class="tiny"><b>Pascuala</b><span>America</span></div>
      </div>

      <!-- SUN -->
      <div class="dayc">
        <h3 class="dayname">Sunday</h3>
        <div class="daydate">August 23</div>
        <div class="daytag">Immediate family only.</div>

        <div class="group" data-who="both">
          <div class="who">Gloria + Antonio</div>
          <div class="item b-rest">
            <div class="t">Morning</div>
            <div class="a">Slow Start</div>
            <div class="c">Nothing scheduled.</div>
          </div>
          <div class="item b-family">
            <div class="t">Midday</div>
            <div class="a">One Family Meal</div>
            <div class="c">Home &middot; simple.</div>
          </div>
        </div>

        <div class="group" data-who="gloria">
          <div class="who g">Gloria</div>
          <div class="item b-family">
            <div class="t">Afternoon</div>
            <div class="a">Time with America</div>
            <div class="c">Brother covers Pascuala.</div>
          </div>
        </div>

        <div class="group" data-who="both">
          <div class="who">Gloria + Antonio</div>
          <div class="item b-rest">
            <div class="t">Evening</div>
            <div class="a">Rest</div>
          </div>
        </div>

        <div class="tiny"><b>Pascuala</b><span>America + brothers</span></div>
      </div>

      <!-- MON -->
      <div class="dayc">
        <h3 class="dayname">Monday</h3>
        <div class="daydate">August 24</div>
        <div class="daytag">The family gathering.</div>

        <div class="group" data-who="gloria">
          <div class="who g">Gloria</div>
          <div class="item b-family">
            <div class="t">Morning</div>
            <div class="a">Family Time</div>
            <div class="c">Pascuala + America.</div>
          </div>
        </div>

        <div class="group" data-who="both">
          <div class="who">Gloria + Antonio</div>
          <div class="item b-guest">
            <div class="t">Afternoon</div>
            <div class="a">Arrivals</div>
            <div class="c">Andree + family &middot; Alex.</div>
          </div>
          <div class="item b-family">
            <div class="t">5:30 <span class="ap">PM</span></div>
            <div class="a">Family Dinner</div>
            <div class="c">Home &middot; casual &middot; catered.</div>
            <div class="mini">Hosted &mdash; the one meal we pay for</div>
          </div>
        </div>

        <div class="group" data-who="antonio">
          <div class="who a">Antonio</div>
          <div class="item b-guest">
            <div class="t">After Dinner</div>
            <div class="a">Alex + Andree</div>
            <div class="c">Brother time.</div>
          </div>
        </div>

        <div class="group" data-who="gloria">
          <div class="who g">Gloria</div>
          <div class="item b-rest">
            <div class="t">Evening</div>
            <div class="a">Pascuala + America</div>
            <div class="c">Relax.</div>
          </div>
        </div>

        <div class="tiny"><b>Arriving</b><span>Andree + wife + child &middot; Alex</span></div>
        <div class="tiny"><b>Pascuala</b><span>America</span></div>
      </div>

      <!-- TUE -->
      <div class="dayc">
        <h3 class="dayname">Tuesday</h3>
        <div class="daydate">August 25</div>
        <div class="daytag">Flex. Protect the open time.</div>

        <div class="group" data-who="gloria">
          <div class="who g">Gloria</div>
          <div class="item b-bride">
            <div class="t">Late Morning</div>
            <div class="a">Wedding Prep + Packing</div>
          </div>
          <div class="item b-family">
            <div class="t">Afternoon</div>
            <div class="a">Pascuala + America</div>
            <div class="c">Easy pace.</div>
          </div>
        </div>

        <div class="group" data-who="antonio">
          <div class="who a">Antonio</div>
          <div class="item b-guest">
            <div class="t">Midday</div>
            <div class="a">Coffee with Ysolina</div>
            <div class="c">Casual &middot; short.</div>
            <div class="mini">Pay own way</div>
          </div>
        </div>

        <div class="group" data-who="both">
          <div class="who">Gloria + Antonio</div>
          <div class="item b-rest">
            <div class="t">Evening</div>
            <div class="a">Quiet at Home</div>
            <div class="c">Pack. No hosted dinner.</div>
          </div>
        </div>

        <div class="tiny"><b>Arriving</b><span>Ysolina (approx.)</span></div>
      </div>
    </div>
  </section>

  <!-- ============ NYC TRANSITION ============ -->
  <section class="band" data-loc="nyc">
    <div class="band-head">
      <h2>NYC &middot; Transition</h2>
      <span class="loc">August 26&ndash;27</span>
    </div>

    <div class="row r2">
      <!-- WED -->
      <div class="dayc">
        <h3 class="dayname">Wednesday</h3>
        <div class="daydate">August 26</div>
        <div class="daytag">Travel day &mdash; chosen over Thursday so Pascuala gets a full day to recover.</div>

        <div class="group" data-who="gloria">
          <div class="who g">Gloria</div>
          <div class="item b-rest">
            <div class="t">Morning</div>
            <div class="a">Breakfast + Finish Packing</div>
          </div>
          <div class="item b-family">
            <div class="t">Mid-Morning</div>
            <div class="a">DC &rarr; NYC</div>
            <div class="c">With Pascuala + America.</div>
          </div>
          <div class="item b-family">
            <div class="t">Afternoon</div>
            <div class="a">Hotel + Settle In</div>
            <div class="c">Get Pascuala comfortable.</div>
          </div>
        </div>

        <div class="group" data-who="antonio">
          <div class="who a">Antonio</div>
          <div class="item b-guest">
            <div class="t">Daytime</div>
            <div class="a">Aliosha + Daughter</div>
            <div class="c">Already in NYC &middot; own plans.</div>
          </div>
          <div class="item b-guest">
            <div class="t">Afternoon</div>
            <div class="a">Alex &middot; Andree + Family</div>
            <div class="c">As they land.</div>
          </div>
        </div>

        <div class="group" data-who="both">
          <div class="who">Gloria + Antonio</div>
          <div class="item b-family">
            <div class="t">Late Afternoon</div>
            <div class="a">Daughter + Grandchildren</div>
            <div class="c">Family time. Not an event.</div>
          </div>
          <div class="item b-rest">
            <div class="t">Evening</div>
            <div class="a">Easy Dinner Near the Hotel</div>
            <div class="c">Room service or takeout is fine.</div>
          </div>
        </div>

        <div class="note"><b>Protect</b><span>No group dinner. Arrivals are not invitations.</span></div>
        <div class="tiny"><b>NYC today</b><span>Daughter + family &middot; Andree + family &middot; Alex &middot; Aliosha + daughter &middot; Sofia + Kelhi</span></div>
        <div class="tiny"><b>Pascuala</b><span>America</span></div>
      </div>

      <!-- THU -->
      <div class="dayc">
        <h3 class="dayname">Thursday</h3>
        <div class="daydate">August 27</div>
        <div class="daytag">The last open day. Keep it spacious.</div>

        <div class="group" data-who="both">
          <div class="who">Gloria + Antonio</div>
          <div class="item b-rest">
            <div class="t">Morning</div>
            <div class="a">Breakfast Together</div>
          </div>
        </div>

        <div class="group" data-who="gloria">
          <div class="who g">Gloria</div>
          <div class="item b-bride">
            <div class="t">Late Morning &ndash; Afternoon</div>
            <div class="a">Ximena + Wedding Needs</div>
            <div class="c">Her list, her pace.</div>
          </div>
        </div>

        <div class="group" data-who="antonio">
          <div class="who a">Antonio</div>
          <div class="item b-guest">
            <div class="t">Midday</div>
            <div class="a">Alex &middot; Andree &middot; Ysolina</div>
            <div class="c">Catch up before the weekend.</div>
          </div>
        </div>

        <div class="group" data-who="both">
          <div class="who">Gloria + Antonio</div>
          <div class="item b-family">
            <div class="t">Afternoon</div>
            <div class="a">Daughter + Grandchildren</div>
            <div class="c">Unhurried family time.</div>
          </div>
          <div class="item b-family">
            <div class="t">Late Afternoon</div>
            <div class="a">Family with Pascuala</div>
            <div class="c">Brothers + Valeska arrive.</div>
          </div>
          <div class="item b-rest">
            <div class="t">Evening</div>
            <div class="a">Casual &middot; Flexible</div>
            <div class="c">If family gathers naturally, fine.</div>
          </div>
        </div>

        <div class="note"><b>Protect</b><span>No hosted dinner. No family reunion.</span></div>
        <div class="tiny"><b>NYC today</b><span>Brothers &middot; Valeska &middot; Ysolina &middot; Betty</span></div>
        <div class="tiny"><b>Pascuala</b><span>America + brothers</span></div>
      </div>
    </div>
  </section>

  <!-- ============ WEDDING WEEKEND ============ -->
  <section class="band" data-loc="nyc">
    <div class="band-head">
      <h2>Wedding Weekend</h2>
      <span class="loc">August 28&ndash;30 &middot; New York City</span>
    </div>

    <div class="row r3">
      <!-- FRI -->
      <div class="dayc">
        <h3 class="dayname">Friday</h3>
        <div class="daydate">August 28</div>
        <div class="daytag">Rehearsal, then straight into celebrating.</div>

        <div class="group" data-who="gloria">
          <div class="who g">Gloria</div>
          <div class="item b-bride">
            <div class="t">11:00 <span class="ap">AM</span></div>
            <div class="a">Bridal Luncheon</div>
            <div class="p">The Plaza</div>
            <div class="c">Pascuala + America included.</div>
          </div>
          <div class="item b-bride">
            <div class="t">After Luncheon</div>
            <div class="a">Getting Ready with Ximena</div>
          </div>
        </div>

        <div class="group" data-who="antonio">
          <div class="who a">Antonio</div>
          <div class="item b-rest">
            <div class="t">Midday</div>
            <div class="a">Open</div>
            <div class="c">Family or friends as it happens.</div>
          </div>
        </div>

        <div class="group" data-who="both">
          <div class="who">Gloria + Antonio</div>
          <div class="item b-bride">
            <div class="t">4:00 <span class="ap">PM</span></div>
            <div class="a">Ceremony Rehearsal</div>
            <div class="p">St. Patrick&rsquo;s Cathedral</div>
          </div>
          <div class="item b-bride">
            <div class="t">5:30 <span class="ap">PM</span></div>
            <div class="a">Post-Rehearsal Cocktails</div>
            <div class="p">Bar 65</div>
          </div>
          <div class="item b-bride">
            <div class="t">7:00 &ndash; 10:00 <span class="ap">PM</span></div>
            <div class="a">Welcome Party</div>
            <div class="c">Seeing everyone here counts.</div>
          </div>
        </div>

        <div class="note"><b>Priority</b><span>Ximena. No separate plans with arriving guests.</span></div>
        <div class="tiny"><b>Arriving</b><span>Mili &middot; Mayra</span></div>
        <div class="tiny"><b>Pascuala</b><span>America</span></div>
      </div>

      <!-- SAT -->
      <div class="dayc">
        <h3 class="dayname">Saturday</h3>
        <div class="daydate">August 29</div>
        <div class="daytag">Ximena &amp; Andy&rsquo;s wedding day.</div>

        <div class="group" data-who="gloria">
          <div class="who g">Gloria</div>
          <div class="item b-bride">
            <div class="t">7:45 <span class="ap">AM</span></div>
            <div class="a">Arrive &amp; Change</div>
            <div class="p">The Plaza</div>
            <div class="c">Hair and makeup begin at 8:00.</div>
          </div>
          <div class="item b-bride">
            <div class="t">Morning</div>
            <div class="a">Getting Ready with Ximena</div>
          </div>
        </div>

        <div class="group" data-who="both">
          <div class="who">Gloria + Antonio</div>
          <div class="item b-bride">
            <div class="t">1:45 &ndash; 2:30 <span class="ap">PM</span></div>
            <div class="a">Family Photos</div>
          </div>
          <div class="item b-bride">
            <div class="t">3:15 <span class="ap">PM</span></div>
            <div class="a">Leave with Ximena</div>
            <div class="c">To St. Patrick&rsquo;s.</div>
          </div>
          <div class="item b-bride">
            <div class="t">4:00 &ndash; 5:00 <span class="ap">PM</span></div>
            <div class="a">Ceremony</div>
            <div class="p">St. Patrick&rsquo;s Cathedral</div>
          </div>
          <div class="item b-bride">
            <div class="t">5:30 <span class="ap">PM</span></div>
            <div class="a">Cocktail Hour</div>
            <div class="p">The Plaza</div>
          </div>
          <div class="item b-bride">
            <div class="t">7:00 <span class="ap">PM</span></div>
            <div class="a">Reception</div>
          </div>
          <div class="item b-bride">
            <div class="t">During Dinner</div>
            <div class="a">Blessing &middot; Toasts &middot; Parent Dances</div>
            <div class="c">Exact times per the official timeline.</div>
          </div>
          <div class="item b-bride">
            <div class="t">11:00 <span class="ap">PM</span></div>
            <div class="a">Reception Ends</div>
          </div>
          <div class="item b-bride">
            <div class="t">11:00 <span class="ap">PM</span> &ndash; 1:00 <span class="ap">AM</span></div>
            <div class="a">Hora Loca</div>
          </div>
        </div>

        <div class="note"><b>Today only</b><span>Be with Ximena. No responsibility to entertain guests.</span></div>
        <div class="tiny"><b>Pascuala</b><span>America stays with her &middot; brothers assist &middot; she leaves when tired and America goes with her &middot; do not assume Hora Loca.</span></div>
      </div>

      <!-- SUN -->
      <div class="dayc">
        <h3 class="dayname">Sunday</h3>
        <div class="daydate">August 30</div>
        <div class="daytag">One more toast before goodbye.</div>

        <div class="group" data-who="both">
          <div class="who">Gloria + Antonio</div>
          <div class="item b-rest">
            <div class="t">Morning</div>
            <div class="a">Easy Morning</div>
          </div>
          <div class="item b-guest">
            <div class="t">10:00 <span class="ap">AM</span> &ndash; 12:00 <span class="ap">PM</span></div>
            <div class="a">Farewell Brunch</div>
            <div class="p">Quality Bistro</div>
            <div class="c">The one place to catch everyone.</div>
          </div>
          <div class="item b-rest">
            <div class="t">Afternoon</div>
            <div class="a">Rest &middot; Family &middot; Flex</div>
            <div class="c">No formal plans.</div>
          </div>
        </div>

        <div class="tiny"><b>Find at brunch</b><span>Florida friends &middot; Betty, Mili + Mayra &middot; Aliosha + daughter &middot; anyone missed this week</span></div>
        <div class="note"><b>Protect</b><span>No mandatory Sunday dinner.</span></div>
      </div>
    </div>
  </section>

  <footer>
    <div class="k">Protect the Week</div>
    <div class="protect">
      <div><em>Mon</em>Main hosted family gathering</div>
      <div><em>Wed</em>No group dinner</div>
      <div><em>Thu</em>No hosted dinner</div>
      <div><em>Fri</em>Ximena + wedding</div>
      <div><em>Sat</em>Ximena + wedding</div>
      <div><em>Sun</em>No mandatory dinner</div>
    </div>
    <p>Meaningful time &gt; equal time.</p>
  </footer>

</div>

<script>
  var state = { who: 'everyone', loc: 'all' };

  function apply(){
    document.querySelectorAll('.group').forEach(function(g){
      var w = g.dataset.who;
      var show = state.who === 'everyone' || w === 'both' || w === state.who;
      g.hidden = !show;
    });

    document.querySelectorAll('.dayc').forEach(function(d){
      var visible = d.querySelectorAll('.group:not([hidden])').length;
      var empty = d.querySelector('.empty');
      if(!visible){
        if(!empty){
          empty = document.createElement('div');
          empty.className = 'empty';
          empty.textContent = 'Nothing scheduled.';
          d.appendChild(empty);
        }
        empty.hidden = false;
      } else if(empty){
        empty.hidden = true;
      }
    });

    document.querySelectorAll('section.band').forEach(function(s){
      s.hidden = !(state.loc === 'all' || s.dataset.loc === state.loc);
    });
  }

  function wire(setId, key){
    document.getElementById(setId).addEventListener('click', function(e){
      var btn = e.target.closest('.btn');
      if(!btn) return;
      state[key] = btn.dataset[key];
      this.querySelectorAll('.btn').forEach(function(b){
        b.setAttribute('aria-pressed', String(b.dataset[key] === state[key]));
      });
      apply();
    });
  }

  wire('whoSet','who');
  wire('locSet','loc');
  apply();
</script>
</body>
</html>
