include $(THEOS)/makefiles/common.mk

TWEAK_NAME = Thinner
$(TWEAK_NAME)_FILES = Tweak.xm
$(TWEAK_NAME)_CFLAGS += -fobjc-arc

include $(THEOS_MAKE_PATH)/tweak.mk

after-install::
	install.exec "killall -9 SpringBoard"
	
SUBPROJECTS += thinnerprefs
include $(THEOS_MAKE_PATH)/aggregate.mk
