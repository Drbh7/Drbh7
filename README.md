-- تأكد من تحميل مكتبة MOOSE
env.info("Loading Moose")

-- إنشاء قائمة للتحالف
local MenuCoalition = MENU_COALITION:New(coalition.side.BLUE, "النقاط")

-- دالة لإضافة النقاط
local function AddPoints()
    trigger.action.outText("تم اضافة بعض النقاط !!", 10)
end

-- إضافة خيار إلى القائمة
MENU_COALITION_COMMAND:New(coalition.side.BLUE, "استلام", MenuCoalition, AddPoints)
