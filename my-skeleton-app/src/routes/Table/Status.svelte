<script>
    export let status;
    let bgColor, fgColor, svgFill;
    switch(status.toLowerCase()) {
        case "active":
            bgColor = "bg-green-100";
            fgColor = "text-green-700";
            svgFill = "fill-green-700";
            break
        case "maintenance":
            bgColor = "bg-blue-100";
            fgColor = "text-blue-700";
            svgFill = "fill-blue-700";
            break
        case "inactive":
            bgColor = "bg-yellow-100";
            fgColor = "text-yellow-700";
            svgFill = "fill-yellow-700";
            break
    }
</script>

<div class={`w-fit flex items-center rounded-2xl px-2 ${bgColor} ${fgColor}`}>
    <svg viewBox="0 0 8 8" height="8" xmlns="http://www.w3.org/2000/svg" class={svgFill+" inline-block"}>
        <circle cx="4" cy="4" r="4" fill="inherit" />
    </svg>
    <div class={"px-1 inline-block"}>{status}</div>
</div>