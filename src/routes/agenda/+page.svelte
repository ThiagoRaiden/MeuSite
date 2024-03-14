<script lang="ts">
    import { Calendar } from "@fullcalendar/core";
    import timeGridPlugin from "@fullcalendar/timegrid";
    import ptLocale from "@fullcalendar/core/locales/pt-br";

    /*Duas semanas*/
    function getValidRange(nowDate: Date) {
        let start = new Date(nowDate.getTime());
        start.setDate(start.getDate() - start.getDay());
        let end = new Date(start.getTime());
        end.setDate(end.getDate() + 20);

        return [start, end];
    }
    function calendarAction(node: HTMLElement) {
        const calendarRef = new Calendar(node, {
            plugins: [timeGridPlugin],
            initialView: "timeGridWeek",
            allDaySlot: false,
            locale: ptLocale,
            slotLabelFormat: {
                minute: "2-digit",
                hour: "2-digit",
                meridiem: "short",
            },
            headerToolbar: {
                left: "prev,next",
                center: "title",
                right: "timeGridWeek,timeGridDay",
            },
            validRange: function (nowDate) {
                let [start, end] = getValidRange(nowDate);

                return {
                    start,
                    end,
                };
            },
            events: "https://fullcalendar.io/api/demo-feeds/events.json",
        });
        calendarRef.render();
        return {
            destroy() {
                calendarRef.destroy();
            },
        };
    }
</script>

<div class="h-screen container flex items-center justify-center bg-card ">
    <iframe
    src="https://calendar.google.com/calendar/appointments/schedules/AcZssZ3EJ1b2aKwHRpMGFnmFA8SOzhxyl2OBtU61GB1POo9c4_msS6-P_Fy8BNXPjJJO97vMirzNN13r?gv=true"
    style="border: 0"
    width="100%"
    height="100%"
    frameborder="0"
></iframe>
</div>

