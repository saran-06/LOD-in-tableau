# LOD-in-tableau
INCLUDE-{include[Sub-Category]:AVG([Sales])}
EXCLUDE-{ EXCLUDE [City]: Avg([Sales])}
FIXED-{FIXED [Customer Name]:SUM([Profit])>0}
calculation field-IF [profit_cust]=True
                  THEN "profitable" ELSE"unprofitable" END
